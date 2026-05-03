### Learn the detection phase of incident response operations
The following steps outline ways for security teams to identify potential threats or ongoing attacks within their environment.

#### Review AWS service notifications
- Monitor Health Dashboard for service notifications
- Check Personal Health Dashboard (PHD) for account-specific alerts
- Configure and review Health events in Amazon EventBridge

#### Review AWS CloudTrail logs
- Analyze API activity and management events
- Monitor data events for specific services
- Check for unauthorized or unusual API calls

#### Monitor AWS security service findings
Monitor the findings of services such as 
- AWS Security Hub
- Amazon GuardDuty
- Amazon Macie
- Amazon Inspector
- AWS Config

Examples of interpreting service findings:

If AWS Security Hub shows a high-severity finding where an IAM user successfully created a new access key and modified security group rules within a short timeframe, this could indicate credential compromise requiring immediate investigation.

If Amazon GuardDuty detects an EC2 instance making outbound connections to known cryptocurrency mining pools while also showing unusually high CPU utilization, this could indicate that the instance has been compromised and is being used for cryptojacking, requiring immediate investigation.

#### Analyze AWS CloudWatch alarms
- Monitor application logs in AWS CloudWatch Logs
- Check composite alarms for complex conditions
- Review metric alarms for resource utilization

#### Investigate VPC Flow Logs
- Examine network traffic patterns
- Identify unusual traffic flows
- Look for suspicious IP addresses

#### Demonstration of Detection an alert
Navigate to Amazon GuardDuty to confirm the alert.

![alt text](image-1.png)