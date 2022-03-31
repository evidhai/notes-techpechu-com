- This one onboards data to Kinesis from multiple inputs like
	- Realtime IoT
	- Metrics and Logs
- Stream are divided into ordered shards (say multiple parts)
- Data retention in Kinesis is ==1 day to 7 days == #exam-revise
- #+BEGIN_CAUTION
  #exam-revise 
  Once data into Kinesis can't be deleted manually , it gets auto deleted based on the retention duration
  #+END_CAUTION
- #+BEGIN_TIP
  #exam-revise
  Single Stream can be used by multiple applications 
  #+END_TIP
- How it looks?
  collapsed:: true
	- Shards are ordered sequence
	- ![image.png](../assets/image_1648751130104_0.png)
-