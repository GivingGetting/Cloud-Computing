# cloud-computing
cloud computing practice

What is Cloud Computing?
Cloud computing is the on-demand delivery of compute power, database, storage, applications, and other IT resources via the internet with pay-as-you-go pricing.

What Is Amazon EC2?
Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) cloud. 


Sign Up for AWS

Create an IAM User

Create a Key Pair
  chmod 400 my-key-pair.pem

Create a Virtual Private Cloud (VPC)

Create a Security Group



Launch EC2 Instance from AWS online https://aws.amazon.com
  0. Create EC2 instance
   
Connect to AWS EC2 from local Mac:
  1. --Open Terminal in Mac
  2. ssh -i dliu53-key-pair-central.pem ec2-user@35.183.126.86
  3. sudo yum update -y
  
Action in Docker:
  4. sudo yum install -y docker
  5. sudo service docker start
  6. sudo usermod -a -G docker ec2-user
  7. --log out
  8. --log back in
  9. docker info
  
Create a Docker image of a PHP web application:
  10. --Sign up for a Docker Hub Account https://hub.docker.com
  11. sudo yum install -y git
  12. git clone https://github.com/awslabs/ecs-demo-php-simple-app
  13. cd ecs-demo-php-simple-app
  14. cat Dockerfile
  15. docker build -t dliu53/amazon-ecs-sample .
  16. docker images
  17. docker run -p 80:80 dliu53/amazon-ecs-sample
  18. --now test the public IP of the server 
  
  
  
  
  
  
  






