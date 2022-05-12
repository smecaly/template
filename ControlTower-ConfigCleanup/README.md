
Config Checker Infrastructure Deployment: Template can be used to create the infrastructure for this solution. It will deploy lambda, lambda Iam Role and event rule.

Once the infra is deployed,

Allow access to lambda role from service catalog portfolio so that the lambda can use the service catalog product ID. Go to service catalog portfolio under groups and roles, select the lambda role ( STACKNAME-LambdaFunctionRole-) and add access. Invite an account from AWS Organization. Accept the invited account. once the account accept the invite, it will trigger the lambda function via the event rule.
