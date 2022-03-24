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
	- In-place
		- During deployment the instances will be taken offline
	- Blue / Green
		- Parallel Ec2 will be maintained here
- Deployment settings