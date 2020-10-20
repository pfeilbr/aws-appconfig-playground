# aws-appconfig-playground

learn [AWS AppConfig](https://docs.aws.amazon.com/appconfig/latest/userguide/what-is-appconfig.html)

> create, manage, and quickly deploy application configurations. AWS AppConfig supports controlled deployments to applications of any size and includes built-in validation checks and monitoring. You can use AWS AppConfig with applications hosted on EC2 instances, AWS Lambda, containers, mobile applications, or IoT devices.

## Concepts

* Application (myapp)
* Environment (dev, test, demo, prod)
* Configuration Profile - actual configuration.  text, json, yaml, S3 object, SSM Document, SSM Parameter, CodePipeline
* Deployment

get configuration via cli
```sh
aws appconfig get-configuration \
--application 'app01' \
--environment 'dev' \
--configuration 'config-profile-01' \
--client-id 'test' \
appconfig.json

cat appconfig.json
```

output

![](https://www.evernote.com/l/AAEqjn5qdblEL5J0kWjsMG2g4OkInAN-hOkB/image.png)

Configuration profile source types

![](https://www.evernote.com/l/AAFPtmY9U1tLhL_v42m3BOxd-jtaQ0ZYJBsB/image.png)

Example JSON configuration profile

![](https://www.evernote.com/l/AAG_2LdzxtpK6o_hfXg_hc2Q-ZfMkjGMCGkB/image.png)

Deployment Strategy Types

![](https://www.evernote.com/l/AAEujdNkJthBD7jwMEzwtF6qj0GctFCDsuoB/image.png)

Start Deployment

![](https://www.evernote.com/l/AAH80DpD0MpJILm3IYc6KpR9yPw3nt845c0B/image.png)

Deployment

![](https://www.evernote.com/l/AAGc3YJs7dhBWr2FLWxLN7yOycCdpbI2ybUB/image.png)



## Resources

* [AWS AppConfig Documentation](https://docs.aws.amazon.com/appconfig/latest/userguide/what-is-appconfig.html)
* [Deploying application configuration to serverless: introducing the AWS AppConfig Lambda extension](https://aws.amazon.com/es/blogs/mt/introducing-aws-appconfig-lambda-extension-deploying-application-configuration-serverless/)
* [AWS AppConfig integration with Lambda extensions](https://docs.aws.amazon.com/appconfig/latest/userguide/appconfig-integration-lambda-extensions.html)
* [sessions-with-aws-sam/appconfig-lambda-extensions/README.md](https://github.com/aws-samples/sessions-with-aws-sam/blob/master/appconfig-lambda-extensions/README.md)
* [sthulb/appconfig-demo](https://github.com/sthulb/appconfig-demo)

