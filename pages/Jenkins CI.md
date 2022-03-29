- It is an Opensource CICD tool
- It can replace
	- CodeBuild
	- CodePipeline
	- CodeDeploy
- Things to consider #exam-revise
	- Must be deployed in Master/Slace config
	- Should deploy on Multi AZ Ec2
	- All projects muct contains **Jenkinsfile** -> which tells what action to be performed
	  ^ Similar to ((623f65b9-47e8-4737-9d94-60a76c79303e))
	-
- Architecture options:
	- Can have Master and Slave both at same EC2 instance
	- Can have Master and Slave on seperate EC2 instances
	- #+BEGIN_TIP
	  In some case you can even have more than one master
	  #+END_TIP
- AWS Whitepaper : [Refer](https://d1.awsstatic.com/whitepapers/DevOps/Jenkins_on_AWS.pdf)
- Must known Jenkins plugin #exam-revise
	- #+BEGIN_NOTE
	  Below are just plugin names, don't confuse it with actual AWS services
	  #+END_NOTE
	- Amazon EC2
		- Automatically spins up and down Jenkins slave based on the load
	- AWS CodeBuild
		- It's more serverless way of doing
		- Each run will be like a codebuild and EC2 will be bright down once the run is finished
	- ECS
	- CodePipeline
		- For CodePipeline integration
	- S3
		- To store the [[Artifacts]] in the S3
		-