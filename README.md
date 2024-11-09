# Create docker image containing app and deploy to private ECR using Terraform
- Create a new github repository and Clone the github repository locally.
- Under your local git folder create terraform" folder to store all TF files (backend.tf, compute.tf, provider.tf and variable.tf) use to setup private ECR repository.
- Locate to terraform folder and run below command one by one. After "terraform apply" success, your private ECR repository will create and please check on AWS console online.
- Locate to flask_app folder you should have files created below.
- Test to build docker images locally, make sure you have docker installed. Run the command below, you should be able to curl the website url.
- To push docker image to AWS ECR, enter the command below (You can get this command form AWS->Private ECR repository-> View push commands). Make sure you have AWS CLI installed and AWS Configure on your local computer. Run all the command one by one, you should able to see your docker image uploaded into AWS ECR.
- Clean up your docker image and ECR after successful.
  - Delete docker image - Go to ECR repository folder, select the docker image and delete.
  - Delete ECR repository folder- Back to the terraform folder, enter terraform destroy and it will remove the AWS ECR folder.
