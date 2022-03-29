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
-