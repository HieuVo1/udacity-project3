## How your deployment process works and how the user can deploy changes

1. Make change in source code.
2. Push code to GitHub
3. Create new pull request
4. CodeBuild will build new image and push to ECR if pull request is merged
5. Change deployment config file to use new image
6. Update resource in cluster through running kubectl apply
