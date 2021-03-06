# ecs-cloudwatch-logs
This repository provides the assets referred to in the [blog post on using Amazon ECS and Amazon CloudWatch logs] (http://blogs.aws.amazon.com/application-management/post/TxFRDMTMILAA8X/Send-ECS-Container-Logs-to-CloudWatch-Logs-for-Centralized-Monitoring)

You can use Amazon CloudWatch to monitor and troubleshoot your systems and applications using your existing system, application, and custom log files. You can send your existing log files to CloudWatch Logs and monitor these logs in near real-time.

The container supports an `CW_CONFIG_S3_URL` environment variable (with format, s3://bucket/file), for the CloudWatch configuration file. If not set, the container will fallback to configuration file set in the container's location, `/etc/cloudwatch/awslogs.conf`.
