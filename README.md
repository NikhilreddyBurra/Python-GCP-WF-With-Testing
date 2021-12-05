# Python-GCP-TestingWorkflow
> Here we are creating a workflow to deploy the App to Google Cloud Run Directly.

Steps to Deploy:
1. Create a DOckerfile for the App you want to deploy.
2. Build and test the Dockerfile in locals first.
3. Use `docker build -t <imagename> .`
4. Use `docker run -p <port>:<port> <imagename>`
5. If the App is working perfectly in the Local, deploy the code to the repositroy to trigeer the workflow.
6. You don't need to trigger workflow put the workflow in `.github/workflows/` folder.
7. Create the secrets in GitHub Secrets. Take the variables from GitHub Actions and store in GitHub secrets 