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
	- Stages #exam-revise
		- Application stop
		- Before install
		- Install
		- After Install
		- Application start
	- Appsec hooks - Have a read on [here](https://docs.aws.amazon.com/codedeploy/latest/userguide/reference-appspec-file-structure-hooks.html)
	- Environment variables availablity for hook
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