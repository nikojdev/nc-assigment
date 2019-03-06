# Instructions:
- Clone/Download from repository
- Build the docker image from folder /source (docker build -t notejam-app .)
- Push the image to your AWS ECR Repository
- Upload the CloudFormation template from /templates/cloudformation to your S3 Bucket & Create new stack CloudFormation Stack
- When prompted, enter the desired username & password for DB & enter the URL of your notejam docker image in the AWS ECR  
- Repository (like 12345678.dkr.ecr.us-east-1.amazonaws.com/ecs-iamges/notejam-docker:1.0.0)
  Caution: Input of the username & password is not safe method. This is only intended for demonstration purposes.
- After successful provisioning of the environment, copy the dns from the newly provisioned ALB and paste it to the browser to test
