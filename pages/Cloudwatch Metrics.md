- Metrics provides info on various services.
- eg: CPU utilisation on EC2
- Basic monitoring - for every 5 min (free)
- Detailed monitoring - can get every 1 min (need to pay for it)
- We can get up **15 months ** of logs in cloudwatch #exam-revise
- Metric retention #exam-revise
	- ![image.png](../assets/image_1649698265875_0.png)
- Must known Metrics
  collapsed:: true
	- EC2
	  collapsed:: true
		- #+BEGIN_IMPORTANT
		  RAM info is not available by default need to use custom metrics for that
		  #+END_IMPORTANT
		- CPU utilisation
		- Network IN
		- Network Out
		- EBS
		-
	- EBS
	  collapsed:: true
		- You don't get info on how much free space available need to rely on custom metrics
	-
	-
- # Custom metrics
- Resolution : #exam-revise
  collapsed:: true
	- Standard - data having 1 min granularity (default)
	- High resolution - data at a granularity of 1 second
- [create custom metric](https://docs.aws.amazon.com/cli/latest/reference/cloudwatch/put-metric-data.html) #hands-on
-