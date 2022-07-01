# Demo for testing CDK IaC with TypeScript and Jest

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Useful commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `cdk deploy`      deploy this stack to your default AWS account/region
* `cdk diff`        compare deployed stack with current state
* `cdk synth`       emits the synthesized CloudFormation template

## Run tests

* `npm run test`    perform the jest unit tests

Runs a test in `test/cdk-testing.test.ts` which checks that property `AWS::SQS::Queue` exists in the CDK template which is created during the test. `AWS::SQS::Queue` property is created in `lib/cdk-testing-stack.ts`. The CloudFormation template can be generated manually using CDK CLI with `cdk synth`. CloudFormation template `CdkTestingStack.template.json` is created under `cdk.out` folder