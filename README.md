# template

Config Checker Infrastructure Deployment:
Template can be used to create the infrastructure for this solution. It will deploy lambda, lambda Iam Role and  event rule.

Once the infra is deployed, 
1. We need to allow access to lambda role from service catalog product
2. We need to invite an account from AWS Organization.
3. We need to accept the invited account.

once the account accept the invite, it will trigger the lambda function via the event rule.
