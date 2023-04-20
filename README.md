# JFrog Pipelines Docker Build Task

Docker build JFrog Pipelines task is a sample task written in bash for reference.

## Inputs

- `dockerImage` input has to be provided as DockerImage:DockerImageTag
- `resourceName` is the resource used for Docker build and publish.

## Sample Configuration

Examples are important, here is the sample config which can be used in pipelines.yaml
```yaml
- task: jfrog/docker_build@v0.0.1
  id: docker_build
  input:
    resourceName: "go_app_gitrepo"
    dockerImage: "<JPD_URL>/<ARTIFACTORY_REPOSITORY>/<DOCKER_IMAGE>:<DOCKER_TAG>"
```