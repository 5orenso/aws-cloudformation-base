# AWS Base setup with Cloudformation

An AWS Base setup from scratch with Cloudformation.

This is your basic setup for your VPC, Subnet, Security Group (w/inbound and outbound rules), Internet gateway,
routing table, IAM groups and IAM users.

With this basic setup you are ready to start launching servers and start development og production stuff.

### Initial setup

__This should only be run once!__

```bash
# Create the base setup
$ bash ./bin/create-stack.sh --template base

# Create new iot groups
$ bash ./bin/create-stack.sh --template iam-groups

# Create new iot users
$ bash ./bin/create-stack.sh --template iam-users

```


### Update stack

After every change you can run this command to update the stack.

```bash
# Update the base setup setup
$ bash ./bin/create-stack.sh --template base --update-stack

# Update iot groups
$ bash ./bin/create-stack.sh --template iam-groups

# Update iot users
$ bash ./bin/create-stack.sh --template iam-users

```



## Other Resources

* [AWS Basic setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-base)
* [AWS Server setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-servers)
* [AWS Lambda boilerplate](https://github.com/5orenso/aws-lambda-boilerplate)
* [Automated AWS Lambda update](https://github.com/5orenso/aws-lambda-autodeploy-lambda)
* [AWS API Gateway setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-api-gateway)
* [AWS IoT setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-iot)
