# CI & CD API

This is a basic NestJS application where we focused on CI & CD implementation.

## Actions Steps

1. Checkout code, install node v20, install dependencies and run tests
2. Use [Semantic Release action](https://github.com/cycjimmy/semantic-release-action) to automatize changelog, version and release management
3. Generate tag with first 7 characters from commit SHA to be used on docker image tag
4. Setup AWS credentials that will be used to push the docker image to [AWS ECR](https://aws.amazon.com/ecr/) and deploy the API to [AWS App Runner](https://aws.amazon.com/apprunner/)
5. Build image tags and push them to ECR
6. Deploy the API container on App Runner based on the image created on ECR

### IAC project

This is the project that manages the roles and resources on AWS: https://github.com/lucasnfarias/rocketseat.ci.cd.iac
