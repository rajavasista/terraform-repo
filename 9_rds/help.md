Once you successfully executed terraform apply, ssh on to the new instance using the public ip

    ssh -i <your pem key>  ubuntu@<public ip>

assume root privialges
    sudo -s
update apt-get and install python so to allow us to use python pip. 
    apt-get update
    apt-get install mysql-client

connect to db using below command
    mysql -h <db host name> -u <db username> -p

show databases;
SELECT VERSION();