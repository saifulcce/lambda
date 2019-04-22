# Stop EC2 Instances after Office hours to save cost.

## Notes

### Lambda Function

Be sure to set the Lambda function timeout high enough (i.e. 1 minute) so that it can iterate through every instance in every region.

### CloudWatch Event Rule

Cron expression: `0 19 ? * MON-FRI *`

2:00pm EST (UTC-5) == 07:00pm (19:00) UTC
