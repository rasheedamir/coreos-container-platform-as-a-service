
The AWS CLI signs requests on your behalf.

The CLI stores credentials specified with aws configure in a local file named credentials in a folder named .aws in your home directory. 

For example, the following commands list the contents of the .aws folder:

Linux, OS X, or Unix

$ ls  ~/.aws

Run the command:



Step 1: Install the required tools...

Step 2: Setup & Get AWS Credentials: http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSGettingStartedGuide/AWSCredentials.html

Step 3: Configure aws credentials

run command aws configure

$ aws configure
AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
Default region name [None]: eu-west-1
Default output format [None]: json

Step 4: 

./bin/create-stack.sh -d qbtest.net
