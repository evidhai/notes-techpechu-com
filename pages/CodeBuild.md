- Overview
	- It is elastic and server less service
	- It's AWS equivalent of build tools like Jenkins
	- Uses Docker under the hood (We can also use custom docker images) #exam-revise
	- It's secured : #exam-revise
	  collapsed:: true
		- can be controlled with [[IAM]]
		- Network settings can be played with [[VPC]]
		- [[KMS]] to encrypt build artifcats
		- [[CloudTrail]] to track API calls
- Working flow
	- ![image.png](../assets/image_1647975987455_0.png)
- #exam-revise 
  #+BEGIN_NOTE
  Timeout and Queue timings can be set from 5 minutes to 8 hours. Where as in Lambda we get only max of 15 min runtime
  #+END_NOTE
- buildspec.yaml file overview
	- sample ```
	- version: 0.2
	  
	  phases:
	    install:
	      runtime-versions:
	        java: corretto11
	    pre_build:
	      commands:
		- echo Nothing to do in the pre_build phase...
		    build:
		      commands:
		- echo Build started on `date`
		- mvn install
		    post_build:
		      commands:
		- echo Build completed on `date`
		  artifacts:
		    files:
		- target/messageUtil-1.0.jar
	- version: 0.2
	  
	  phases:
	    install:
	      runtime-versions:
	        java: corretto11
	    pre_build:
	      commands:
		- echo Nothing to do in the pre_build phase...
		    build:
		      commands:
		- echo Build started on `date`
		- mvn install
		    post_build:
		      commands:
		- echo Build completed on `date`
		  artifacts:
		    files:
		- target/messageUtil-1.0.jar