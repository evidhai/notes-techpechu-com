- Overview
  collapsed:: true
	- To Deploy your code/application to multiple EC2 instances
	- As pre-requisite all your EC2 should have code deploy agent running
- Workflow
  collapsed:: true
	- ![image.png](../assets/image_1648145458219_0.png)
	-
- #+BEGIN_IMPORTANT
  - Code deployment can be chained to [[CodePipeline]] 
  - It supports Deployment at Lambda , EC2 , On prime instances , ECS , ASG
  - EC2 instances are grouped by deployment group (dev, test ,prod)
  #+END_IMPORTANT
- Configure CodeDeploy agent at EC2 instance [Refer here](https://docs.aws.amazon.com/codedeploy/latest/userguide/instances-ec2-configure.html) #hands-on
- Deployment types #exam-revise
  collapsed:: true
	- In-place
		- During deployment the instances will be taken offline
	- Blue / Green
		- Parallel Ec2 will be maintained here
		- You need to use ASG for this and one of ELB to be used
- Deployment settings #exam-revise
  collapsed:: true
	- One at a time
		- take one instance offline and perform the deployment at once
	- Half at a time
		- take half of instances (say if you have 4 instances 2 will be done at once) offline and perform the deployment at once
	- All at once
		- All instances will be taken down and deployment will occur
- appspec.yml - deepdive
  collapsed:: true
	- Stages #exam-revise
		- Application stop
		- Before install
		- Install
		- After Install
		- Application start
	- Appsec hooks - Have a read on [here](https://docs.aws.amazon.com/codedeploy/latest/userguide/reference-appspec-file-structure-hooks.html)
	- Environment variables availablity for hook #exam-revise
		- APPLICATION_NAME
			- The name of the application in CodeDeploy that is part of the current deployment (for example, WordPress_App).
		- DEPLOYMENT_ID
			- The ID CodeDeploy has assigned to the current deployment (for example, d-AB1CDEF23).
		- DEPLOYMENT_GROUP_NAME
			- The name of the deployment group in CodeDeploy that is part of the current deployment (for example, WordPress_DepGroup).
		- DEPLOYMENT_GROUP_ID
			- The ID of the deployment group in CodeDeploy that is part of the current deployment (for example, b1a2189b-dd90-4ef5-8f40-4c1c5EXAMPLE).
		- LIFECYCLE_EVENT
			- The name of the current deployment lifecycle event (for example, AfterInstall).
- #+BEGIN_TIP
  CodeDeploy can be integrated with [[CloudWatch]] followed by CloudWatch events and alarm, also can be pointed to SNS notification
  #+END_TIP
- Rollbacks #exam-revise
  collapsed:: true
	- Refer [here](https://docs.aws.amazon.com/codedeploy/latest/userguide/deployments-rollback-and-redeploy.html)
	- Automatic Rollback
		- Rollback when deployment fail
		- Rollback when alarm thershold are met
			- - Can be configured cloudwatch alarm
	- Manual rollbacks
	- Rollback and redeployment workflow
	- Rollback behavior with existing content
- CodeDeploy on On-premise instance
  collapsed:: true
	- You need one IAM per On-premise instances
		- [Guide](https://docs.aws.amazon.com/codedeploy/latest/userguide/on-premises-instances-register.html) #hands-on
	- #+BEGIN_WARNING
	  #exam-revise 
	  Best practice is to use IAM session ARN to manage instances at large scale
	  For better security use STS to create temp credentials
	  #+END_WARNING
- Deployment Configuration for Lambda #exam-revise
  collapsed:: true
	- Canary
		- - Here initial x % traffic will be shifted to new version and then 100% will be directly shifted on the 2nd increment itself
	- Linear
		- The version swap happens x% by x% (equal % at equal number of interval)
	- All at once
- Deployment Hooks for Lambda deployment
	- Start
	- Before allow traffic
	- Allow Traffic
	- After Allow Traffic
	- End