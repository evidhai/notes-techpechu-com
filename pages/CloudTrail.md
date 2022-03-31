- CloudTrail by default records all events (any action performed by the user)that happens within your account
- Data events #exam-revise
  collapsed:: true
	- We can store all events in S3 or we can trigger [[Lambda]] for which we will be creating Trail and choose respective Data events
	- By default logs stored in S3 bucket are SSE-S3 encrypted
	- can be mapped to [[SNS]]  for every log file delivery
- CloudTrail Logs can be configured to get it delivered to [[CloudWatch Logs]]
- #+BEGIN_IMPORTANT
  
  There is a 15 min delay for CloudTrail to S3 . If you need realtime notification then use [[CloudWatch events]] 
  #+END_IMPORTANT
-