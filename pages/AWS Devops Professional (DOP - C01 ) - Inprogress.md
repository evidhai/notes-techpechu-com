- #+BEGIN_QUOTE
  Study material for AWS devops professional. 
  I will add notes as  Day 1 , 2  .... so that when you refer the notes anytime you can take the timeline as reference !
  #+END_QUOTE
- ## Prerequiste
	- Minimum any one Associate level certificate
	- Pure hands-on and going to need practice , practice so let's get our hands dirty 😊
	- Get your AWS account created
	- Get your AWS CLI setup
- Day wise tracker
	- Day 1
		- ((6238bf86-e7cf-4b09-acb6-89a9bd9e1307))
	- Day 2
		- ((6238bf86-9de5-49b0-8f5f-ab6c7d976ced))
	- Day 3
		- ((6238bf86-0802-4806-b2c6-5a1e0500f084))
	- Day 4
		- ((623a275d-36c2-43eb-b2e5-6612da8ffd3b)) Practiced Hands-on and revised topic for Day 1 - 3
	- Day 5
		- ((6238bf86-06af-45c9-9724-cf8f40badcc2))
	- Day 6
		- ((6241f27e-2baa-4ed5-b069-efe8195f6dab))
	- Day 7
		- ((62434b14-d801-44a9-b621-c1582ce00474))
		- ((623f65b8-4fd2-44e9-bfb7-ff675907fa4c))
	- Day 8
		- Today we played with our hobby project -> way how we actually hosted our blog https://notes.techpechu.com to execute some commands over pipeline!
		- Nothing much but it was fun! Will continue tomorrow
	- Day 9
		- ((6245e567-55a5-4256-bcd3-2ccb2b8c1000))
		- ((6245ee0c-8e48-491d-a887-a68516a7ee01))
	- Day 10
		- ((625464bb-3dcd-4966-a004-f4d6e1c17a5c))
		- ((62546ca6-1ede-4a85-92ed-3002b8086fef))
		-
		-
		-
- # Topic: SDLC Atomation
  collapsed:: true
	- ## CICD Overview
	  id:: 6238bf86-e7cf-4b09-acb6-89a9bd9e1307
	  collapsed:: true
		- ### Continuous Integration
		  collapsed:: true
			- ![image.png](../assets/image_1647885932857_0.png)
		- ### Continuous Delivery vs Deployment
		  id:: 623f65b8-1902-4455-a1a3-09cfb8e46d7e
			- Continuous Delivery
				- When entire deployment till Production occurs with some manual intervention
			- Continuous Deployment
				- No manual intervention at all
		- ### Stacks to focus on
			- [[CodeCommit]]
			  id:: 6238bf86-9de5-49b0-8f5f-ab6c7d976ced
			- [[CodeBuild]]
			  id:: 6238bf86-0802-4806-b2c6-5a1e0500f084
			- [[CodePipeline]]
			  id:: 6241f27e-2baa-4ed5-b069-efe8195f6dab
			- [[CodeStar]]
			  id:: 62434b14-d801-44a9-b621-c1582ce00474
			- [[Elastic Beanstalk]]
			- [[CodeDeploy]]
			  id:: 6238bf86-06af-45c9-9724-cf8f40badcc2
			- [[Jenkins CI]]
			  id:: 623f65b8-4fd2-44e9-bfb7-ff675907fa4c
			- [[Cloudformation]]
		- TODO Whitepaters to read on
			- MUST READ - Blue/Green Deployments on AWS/   https://d1.awsstatic.com/whitepapers/AWS_Blue_Green_Deployments.pdf
			  RECOMMENDED - Practicing Continuous Integration Continuous Delivery on AWS
			      https://d1.awsstatic.com/whitepapers/DevOps/practicing-continuous-integration-continuous-delivery-on-AWS.pdf
			  RECOMMENDED - Jenkins on AWS
			      https://d1.awsstatic.com/whitepapers/DevOps/Jenkins_on_AWS.pdf
			  OPTIONAL - Introduction to DevOps on AWS
			      https://d1.awsstatic.com/whitepapers/AWS_DevOps.pdf
			  OPTIONAL - Development and Test on AWS
			      https://d1.awsstatic.com/whitepapers/aws-development-test-environments.pdf
		-
	- Reference links
	  collapsed:: true
		- CodeCommit
			- https://www.atlassian.com/git/tutorials/using-branches
			- https://docs.aws.amazon.com/codecommit/latest/userguide/auth-and-access-control-iam-identity-based-access-control.html
			- https://aws.amazon.com/blogs/devops/refining-access-to-branches-in-aws-codecommit/
			- https://docs.aws.amazon.com/codecommit/latest/userguide/how-to-notify.html
			- https://docs.aws.amazon.com/codecommit/latest/userguide/how-to-repository-email.html )
			- https://docs.aws.amazon.com/codecommit/latest/userguide/how-to-notify-lambda.html
			- https://docs.aws.amazon.com/codecommit/latest/userguide/how-to-migrate-repository-existing.html
		- CodeBuild
			- https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html
			- https://docs.aws.amazon.com/codebuild/latest/userguide/samples.html
			- https://docs.aws.amazon.com/codebuild/latest/userguide/sample-docker.html
			- https://aws.amazon.com/blogs/devops/validating-aws-codecommit-pull-requests-with-aws-codebuild-and-aws-lambda/
		- CodeDeploy
			- https://docs.aws.amazon.com/codedeploy/latest/APIReference/API_MinimumHealthyHosts.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/reference-appspec-file-structure-hooks.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/reference-appspec-file-structure-hooks.html#appspec-hooks-server
			- https://docs.amazonaws.cn/en_us/codedeploy/latest/userguide/reference-appspec-file-structure-hooks.html#reference-appspec-file-structure-environment-variable-availability
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/monitoring-cloudwatch-events.html
			- https://aws.amazon.com/blogs/devops/view-aws-codedeploy-logs-in-amazon-cloudwatch-console/
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/monitoring-sns-event-notifications.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/deployments-rollback-and-redeploy.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/deployment-groups-configure-advanced-options.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/instances-on-premises.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/register-on-premises-instance-iam-user-arn.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/register-on-premises-instance-iam-session-arn.html
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/deployment-configurations.html#deployment-configuration-lambda
			- https://docs.aws.amazon.com/codedeploy/latest/userguide/reference-appspec-file-structure-hooks.html#appspec-hooks-lambda
		- CodePipeline
			- https://docs.aws.amazon.com/codepipeline/latest/userguide/reference-pipeline-structure.html#action-requirements
			- https://docs.aws.amazon.com/codepipeline/latest/userguide/best-practices.html#use-cases
			- https://docs.aws.amazon.com/codepipeline/latest/userguide/actions-invoke-lambda-function.html
			- https://docs.aws.amazon.com/codepipeline/latest/userguide/actions-create-custom-action.html
			- https://docs.aws.amazon.com/codepipeline/latest/APIReference/API_PutJobSuccessResult.html
			- https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/continuous-delivery-codepipeline.html
			- https://docs.aws.amazon.com/codepipeline/latest/userguide/tutorials-cloudformation.html
			- https://github.com/aws-samples/codepipeline-nested-cfn
			- https://aws.amazon.com/blogs/devops/implementing-gitflow-using-aws-codepipeline-aws-codecommit-aws-codebuild-and-aws-codedeploy/
		- CodeStar
			- https://docs.aws.amazon.com/codestar/latest/userguide/templates.html
		- Jenkins
			- https://aws.amazon.com/getting-started/projects/setup-jenkins-build-server/
			- https://wiki.jenkins.io/display/JENKINS/Amazon+EC2+Plugin
			- https://aws.amazon.com/blogs/devops/setting-up-a-ci-cd-pipeline-by-integrating-jenkins-with-aws-codebuild-and-aws-codedeploy/
			- https://wiki.jenkins.io/display/JENKINS/AWS+CodeBuild+Plugin
			- https://wiki.jenkins.io/display/JENKINS/Amazon+EC2+Container+Service+Plugin
			- https://wiki.jenkins.io/display/JENKINS/Artifact+Manager+S3+Plugin
			- https://wiki.jenkins.io/display/JENKINS/AWS+CodePipeline+Plugin
- # Topic : Monitoring and Logging
	- [[CloudTrail]]
	  id:: 6245e567-55a5-4256-bcd3-2ccb2b8c1000
	- [[Kinesis]]
	  id:: 6245ee0c-8e48-491d-a887-a68516a7ee01
	- [[Cloudwatch Metrics]]
	  id:: 625464bb-3dcd-4966-a004-f4d6e1c17a5c
	- [[Cloudwatch Alarm]]
	  id:: 62546ca6-1ede-4a85-92ed-3002b8086fef
	- [[Cloudwatch Logs]]
	- [[Cloudwatch unified agent]]
	-
	-
	-
	-
	- Reference links
	  collapsed:: true
		- CloudTrail:
		- https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-log-file-validation-cli.html
		- https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-receive-logs-from-multiple-accounts.html
		- https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-sharing-logs.html
		- CloudWatch:
		- https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch_concepts.html#Metric
		- https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/metrics-collected-by-CloudWatch-agent.html#linux-metrics-enabled-by-CloudWatch-agent
		- https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Counting404Responses.html
		- https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Subscriptions.html
		- https://aws.amazon.com/blogs/big-data/power-data-ingestion-into-splunk-using-amazon-kinesis-data-firehose/
		- https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/SubscriptionFilters.html#FirehoseExample
		- https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/Create-CloudWatch-Events-CloudTrail-Rule.html
		- https://docs.aws.amazon.com/AmazonS3/latest/user-guide/enable-event-notifications.html
		- X-Ray:
		- https://docs.aws.amazon.com/xray/latest/devguide/aws-xray.html
		- https://aws.amazon.com/blogs/devops/using-amazon-cloudwatch-and-amazon-sns-to-notify-when-aws-x-ray-detects-elevated-levels-of-latency-errors-and-faults-in-your-application/
		- Amazon ES:
		- https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_ES_Stream.html
		- Tagging in AWS
		- https://aws.amazon.com/answers/account-management/aws-tagging-strategies/