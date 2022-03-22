- Overview
  collapsed:: true
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