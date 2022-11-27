
# AWS CLI Installation in Linux

## Step 1: Get to know your OS version
```
$ uname -a
Linux ip-172-31-92-233.ec2.internal 4.18.0-372.9.1.el8.x86_64 #1 SMP Fri Apr 15 22:12:19 EDT 2022 x86_64 x86_64 x86_64 GNU/Linux
```
## Step 2: Install the packages curl and unzip
```
$ sudo yum install curl unzip -y
```
## Step 3: Download the AWS CLI package
```
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
```
## Step4: Extract the folder from the zip file
```
$ unzip awscliv2.zip
```
## Step5: Execute the install file
```
$ sudo ./aws/install
```
## Step6: Now check the AWS CLI version
```
$ /usr/local/bin/aws --version
aws-cli/2.8.12 Python/3.9.11 Linux/5.10.144-127.601.amzn2.x86_64 exe/x86_64.amzn.2 prompt/off
$ aws --version
aws-cli/2.8.4 Python/3.9.11 Linux/4.18.0-372.9.1.el8.x86_64 exe/x86_64.rhel.8 prompt/off
```
## Step 7: Now, its time to configure AWS CLI. Get the KEY ID and Secret Access key from the user details in AWS Console.
```
$ aws configure
AWS Access Key ID [None]: xxxxxxxxxxxxxxx
AWS Secret Access Key [None]: xxxxxxxxxxxxxxxx
Default region name [None]: us-west-2
Default output format [None]: json
```


```
Happy to receive your feedbacks ...
'``
