# Chatbot App

> short description

> any note if availabe

> sample image of our app

> architecture details

> architectre image

## Architecture details

> short description

> another short description 

AWS Service | Usage Overview | Focused Point
--- | --- | ---

## Supported Regions

> Example:
The Retail Demo Store has been tested in the AWS regions indicated in the deployment instructions below. Additional regions may be supported depending on [service availability](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/) and having the Retail Demo Store's deployment resources staged to an S3 bucket in the targeted region.

## Getting Started

> IMPORTANT NOTE:

> What Purpose, cross country, applicable laws

> if someone is developer

> Deployment notice (Example):
To get the Retail Demo Store running in your own AWS account, follow these instructions. If you are attending an AWS-led event where temporary AWS accounts are provided, this has likely already been done for you already. Check with your event administrators.

## Step 1 - Get an AWS Account

If you do not have an AWS account, please see [How do I create and activate a new Amazon Web Services account?](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)

## Step 2 - Log into the AWS Console

Log into the [AWS console](https://console.aws.amazon.com/) if you are not already. 

Note: If you are logged in as an IAM user, ensure your account has permissions to create and manage the necessary resources and components for this application.

## Step 3 - Deploy to your AWS Account

> Example
The following CloudFormation launch options will set the deployment approach to "CodeCommit". You can ignore the GitHub related template parameters. After clicking one of the Launch Stack buttons below, follow the procedures to launch the template.

With this deployment option, the CloudFormation template will import the Retail Demo Store source code into a CodeCommit repository in your account and setup CodePipeline to build and deploy into ECS from that respository.

> Example


Region name | Region code | Launch
--- | --- | ---
US East (N. Virginia) | us-east-1 | [![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://google.com)
US West (Oregon) | us-west-2 | [![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://google.com)
Europe (Ireland) | eu-west-1 | [![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://google.com)

The CloudFormation deployment will take 20-30 minutes to complete.

## Step 4 - Using the Retail Demo Store Web Application

> Examples
Once you launch the CloudFormation stack, all of the services will go through a build and deployment cycle and deploy the Retail Demo Store. 

Compiling and deploying the web UI application and the services it uses can take some time. You can monitor progress in CodePipeline. Until this completes, you may see a Sample Application when accessing the public WebUI URL.

You can find the URL for the Retail Demo Store Web UI in the Outputs of your main CloudFormation stack (called `retaildemostore` unless you changed that option in the steps above). 

Look for the "WebURL" output parameter.

You can read more [detailed instructions on how to demo the Retail Demo Store in the Demo section at the end of this document](#delivering-a-demo-of-the-retail-demo-store).

# Developer Instructions

If you're interested in contributing enhancements, features, or fixes to the Retail Demo Store, please see the [Developer Instructions](./Developer-Instructions.md) for details on how to setup your local environment and deployment environment.

# Delivering a Demo of the Retail Demo Store

Once you have deployed the Retail Demo Store, you may want to walk through the demonstration guide to learn how to show the features the Retail Demo Store provides.

The intent of the Retail Demo Store is to 1) provide a tool to demonstrate the capabilities of key AWS services for retail, eCommerce, and digital marketing use-cases and 2) provide a platform for individual AWS customers to step through workshops and AWS internal teams to deliver customer-facing workshops, Immersion Days, hackathons, and similar types of events.

1) [Creating a Retail Demo Store account](./documentation/1-Creating-account.md)
2) [Personalized Experience](./documentation/2-Personalization.md)

# Known Issues

* The application was written for demonstration purposes and not for production use.
* You currently cannot deploy this project multiple times in the same AWS account and the same region. However, you can deploy the project into separate regions within the same AWS account.
* Make sure your CloudFormation stack name uses all lowercase letters.
* Currently only tested in the AWS regions provided in the deployment instructions above. The only limitation for deploying into other regions is [availability of all required services](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/).

# Reporting Bugs

If you encounter a bug, please create a new issue with as much detail as possible and steps for reproducing the bug. See the [Contributing Guidelines](./CONTRIBUTING.md) for more details.

# License

This sample code is made available under a modified MIT license. See the LICENSE file.

