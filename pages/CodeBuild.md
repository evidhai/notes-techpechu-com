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
- buildspec.yaml file Deep dive
	- sample
	  collapsed:: true
		- ```
		  version: 0.2
		  
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
		      finally:
		        - echo Whoohoo
		    post_build:
		      commands:
		        - echo Build completed on `date`
		  artifacts:
		    files:
		      - target/messageUtil-1.0.jar
		  ```
	- 4 phases which can define #exam-revise
	  collapsed:: true
		- 1. install
		  2. pre-build
		  3. build
		  4. post-build
	- commands vs finally
	  collapsed:: true
		- Finally is executed post commands and it will be executed for sure even if command initialised any error on execution
		- #+BEGIN_TIP
		  Finally is used to do any cleanup before terminating
		  #+END_TIP
	- Reference for buildspec syntax [here](https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html#build-spec-ref-syntax)
	- Use case based samples can be found [here](https://docs.aws.amazon.com/codebuild/latest/userguide/use-case-based-samples.html) #hands-on