# News Demo Setup

This repository is set up with GitHub Workflow. There are 2 workflows:

* News Demo CI
  * This runs on pull request and new commits pushed to main branch. 
  * This will build, test and lint the code in commit or pull request.
  * This will run only on code changes and not on files which are not code related for eg. README.md

* Create and publish a Docker image to ghcr
  * This runs only on new commits pushed to main branch.
  * This will build the docker images using the latest code and push to ghcr registry.
  * This will also run only on code changes and not on files which are not code related for eg. README.md

To run the application on a kubernetes cluster, please check the instructions [here](./README.md#deploying-on-kubernetes-cluster)

### Improvements

* Integrating a kubernetes cluster with GitHub workflow so that we can deploy the latest code on the cluster