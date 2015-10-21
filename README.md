
The AWS CLI signs requests on your behalf.

The CLI stores credentials specified with aws configure in a local file named credentials in a folder named .aws in your home directory. 

For example, the following commands list the contents of the .aws folder:

Linux, OS X, or Unix

$ ls  ~/.aws

Run the command:

Step 1: Install the required tools...

a. jq
curl http://stedolan.github.io/jq/download/linux64/jq -o /usr/local/bin/jq
chmod +x /usr/local/bin/jq



Step 2: Setup & Get AWS Credentials: http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSGettingStartedGuide/AWSCredentials.html

Step 3: Configure aws credentials

run command aws configure

$ aws configure
AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
Default region name [None]: eu-west-1
Default output format [None]: json

Step 4: 

./bin/create-stack.sh -d cp.qbtest.net


INFO: generating a new key pair in stacks/cpqbtestnet/cp.pem
./bin/create-stack.sh: line 111: warning: here-document at line 106 delimited by end-of-file (wanted `!')
./bin/create-stack.sh: line 111: warning: here-document at line 106 delimited by end-of-file (wanted `!')
{
    "StackId": "arn:aws:cloudformation:eu-west-1:838562712530:stack/cpqbtestnet/79893260-7694-11e5-9944-50d5026f660a"
}
INFO: create in progress. sleeping 15 seconds...
INFO: create in progress. sleeping 15 seconds...
INFO: create in progress. sleeping 15 seconds...
INFO: create in progress. sleeping 15 seconds...
INFO: create in progress. sleeping 15 seconds...
INFO: create in progress. sleeping 15 seconds...
INFO: create in progress. sleeping 15 seconds...
INFO: create in progress. sleeping 15 seconds...

CoreOSServerAutoScale	52.19.101.215	172.31.5.2
CoreOSServerAutoScaleConsulServer	52.30.21.77	172.31.19.214
CoreOSServerAutoScaleConsulServer	52.30.49.231	172.31.4.177
CoreOSServerAutoScaleConsulServer	52.30.64.100	172.31.33.109

ssh-add stacks/cpqbtestnet/cp.pem
ssh core@52.30.103.198

to view consul:
ssh -A -L 8500:172.31.19.214:8500 core@52.30.64.100