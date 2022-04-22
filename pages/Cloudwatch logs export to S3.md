- Method 1:
	- For one time you can get it exported manually [hands-on guide](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/S3ExportTasksConsole.html) #hands-on
- Method 2:
	- Wrtie a Lambda code to use method 1 api
	- Use Cloudwatch events to trigger Lambda and get the logs exported
-
- Method 3:
	- Raltime processing of Log Data with subscription
	- We can send realtime data to end locations such as [[Kinesis Streams]] [[Kinesis Firehose]] [[Lambda]]
	- #+BEGIN_CAUTION
	  Subscription to Kinesis can't be done via Console and need to rely on CLI to achieve
	  #+END_CAUTION
		- ![image.png](../assets/image_1650650309933_0.png){:height 289, :width 444}
	- [Hands-on guide](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/SubscriptionFilters.html) #hands-on
-