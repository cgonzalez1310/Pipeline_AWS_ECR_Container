# Pipeline_AWS_ECR_Container
pipeline for create a docker image and push it to AWS ECR repository


First: Authenticate Docker (running in self hosted) with aws ECR
second: self hosted EC2 build the docker image and create a tag for each image to a unique identifier using the GITHUB_SHA::7 
thrid: tag and push docker image to AWS ECR and export the fill docker image URI as environment variable for next uses "$GITHUB_ENV"
four: 
