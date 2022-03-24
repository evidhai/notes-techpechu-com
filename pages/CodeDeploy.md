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
  - It supports Deployment at Lambda and EC2
  - EC2 instances are grouped by deployment group (dev, test)
  #+END_IMPORTANT