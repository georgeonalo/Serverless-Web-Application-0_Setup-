# Setup

## AWS Account

In order to complete this project, you'll need an AWS account and access to create AWS Identity and Access Management (IAM), Amazon Cognito, AWS Lambda, Amazon S3, Amazon API Gateway, AWS Amplify Console, Amazon DynamoDB, and AWS Cloud9 resources within that account.

The code and instructions in this project assume only one participant is using a given AWS account at a time. If you attempt sharing an account with another participant, you will encounter naming conflicts for certain resources. You can work around this by either using a suffix in your resource names or using distinct Regions, but the instructions do not provide details on the changes required to make this work.

Use a personal account or create a new AWS account for this workshop rather than using an organization's account to ensure you have full access to the necessary services and to ensure you do not leave behind any resources from the project.

### AWS Cloud9 IDE

AWS Cloud9 is a cloud-based integrated development environment (IDE) that lets you write, run, and debug your code with just a browser. It includes a code editor, debugger, and terminal. Cloud9 comes pre-packaged with essential tools for popular programming languages and the AWS Command Line Interface (CLI) pre-installed so you don’t need to install files or configure your laptop for this workshop. Your Cloud9 environment will have access to the same AWS resources as the user with which you logged into the AWS Management Console.

Take a moment now and setup your Cloud9 development environment.

#### ✅ Step-by-step Instructions

1. Go to the AWS Management Console, click Services then select Cloud9 under Developer Tools.

2. Click Create environment.

3. Enter Development into Name and optionally provide a Description.

4. Click Next step.

5. You may leave Environment settings at their defaults of launching a new t2.micro EC2 instance which will be paused after 30 minutes of inactivity.

6. Click Next step.

7. Review the environment settings and click Create environment. It will take several minutes for your environment to be provisioned and prepared.

8. Once ready, your IDE will open to a welcome screen. Below that, you should see a terminal prompt.

You can run AWS CLI commands in here just like you would on your local computer. Verify that your user is logged in by running aws sts get-caller-identity.

aws sts get-caller-identity

You'll see output indicating your account and user information:

ec2-user:~/environment $ aws sts get-caller-identity

{

    "Account": "123456789012",
    
    "UserId": "AKIAI44QH8DHBEXAMPLE",
    
    "Arn": "arn:aws:iam::123456789012:user/Alice"
    
}

Keep your AWS Cloud9 IDE opened in a tab throughout this workshop.

##### ⭐ Tips

💡 Keep an open scratch pad in Cloud9 or a text editor on your local computer for notes. When the step-by-step directions tell you to note something such as an ID or Amazon Resource Name (ARN), copy and paste that into the scratch pad.

###### Next

✅ Proceed to the first module,([[staticWeb Hosting](https://github.com/georgeonalo/Serverless-Web-Application-1_StaticWebHosting-)]): ([https://github.com/georgeonalo/Serverless-Web-Application-1_StaticWebHosting-]), wherein you'll deploy a static web site via AWS Amplify Console.
