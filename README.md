# Azure DevOps PR branch auto-update

A pipeline to auto-update PRs with the latest changes whenever something is pushed into the base branch.

It was primarily created for Azure DevOps which, unlike Github, lacks the "Update branch" button on the PR's web UI page.

# How to use

1. Navigate to the Azure DevOps organization/project you'd like to add the pipeline to
2. [Grant the following permissions to the build service](https://learn.microsoft.com/en-us/azure/devops/pipelines/scripts/git-commands?view=azure-devops&tabs=yaml#grant-version-control-permissions-to-the-build-service):
   * Contribute: Allow
   * Contribute to pull requests: Allow
3. Copy the [pipeline file](/azure-pipelines.yaml) into your repo
4. Create a new pipeline using this file
5. Done 🎉
