# terraform-repo

ssh-keygen -t rsa -b 2048 -f ~/.ssh/devopsmonks.pem -q -P ''
chmod 400 ~/.ssh/devopsmonks.pem & ssh-keygen -y -f ~/.ssh/devopsmonks.pem > ~/.ssh/devopsmonks.pub



Manual installation: Download from here: https://www.terraform.io/downloads.html
for windows: in powershell admin console "choco install terraform"
for mac use "brew install terraform"

https://www.terraform.io/docs/providers/aws/index.html#shared-credentials-file


create a new user terraform_user in aws iam, set access type programmatic access

assign policy with admin access

aws configure or
- mkdir .aws
- create a file with name 'credentials' - vi credentials
- and then copy paste below lines in .aws/credentials file

[terraform]
aws_access_key_id = xxxxxxxxxxxxxxxxxxx
aws_secret_access_key = xxx/xxxxxxxxxxxxx/xxxx


here terraform is the profile in AWS ..
