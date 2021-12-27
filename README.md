# build-and-push-docker-image-via-github-action

Using this github workflow you will be able to build and test your maven application. As well as you will containerize your application. Means a docker images will be created and pushed to your dockerhub accout.

The main use case of this Workflow is you can call the github worklfow/pipeline present in the diffeant repository.

Example 1: "Java CI with Maven" can trigger the "workflow-2" after  the particular step .But here the workflow-2 is present in the same repo.

Example 2: To call workflow which present in the differant you can use commented code. And just need to add the differant-repo workflow.yml into your second repo. As my second repo is "Hello-World" And you can specify your own steps in that workflow you required.

Here is the link of my second repo you can check it out https://github.com/sakshigawande12/HelloWorld/blob/pull-request-using-gh-actions/.github/workflows/scala.yml


Note: You just need to add the following secrets to you repo

1. DOCKERHUB_USERNAME
2. DOCKERHUB_PASSWORD

To work this workflow successully your workflow has to be present on default branch.

