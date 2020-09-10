# sam-golang-example-20200801

## install sam

```
% pip install aws-sam-cli
```

## sam init

```
% sam init --runtime go1.x --name api-example

	SAM CLI now collects telemetry to better understand customer needs.

	You can OPT OUT and disable telemetry collection by setting the
	environment variable SAM_CLI_TELEMETRY=0 in your shell.
	Thanks for your help!

	Learn More: https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-telemetry.html

Which template source would you like to use?
	1 - AWS Quick Start Templates
	2 - Custom Template Location
Choice: 1

Cloning app templates from https://github.com/awslabs/aws-sam-cli-app-templates.git

AWS quick start application templates:
	1 - Hello World Example
	2 - Step Functions Sample App (Stock Trader)
Template selection: 1

-----------------------
Generating application:
-----------------------
Name: api-example
Runtime: go1.x
Dependency Manager: mod
Application Template: hello-world
Output Directory: .

Next steps can be found in the README file at ./api-example/README.md
```

## make

```
% make
```

## local api

```
% sam local start-api
```

## deploy

> To deploy your application for the first time, run the following in your shell:

```
% sam deploy --guided
```

## delete stack

```
% aws cloudformation delete-stack --stack-name <STACK_NAME>
```

(SAM management stacks are not deleted.)
