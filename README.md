# **CICD ADF Databricks**

**This is in extension to this [Project](https://github.com/Mar8el/Azure-e2e-data-engineering-project)
implementing Continuous Integration and Continuous Deployment (CI/CD) pipelines for Azure Data Factory (ADF) and Databricks using GitHub Actions.**

## Workflow:
- CI: Any time when there is a change made to the main branch in either of the folder ADF or Databricks YML file will get triggered accordingly adf_main.yml or db_main.yml
  
- Build: Generate ARM templates, zip notebooks, store as GitHub artifacts.
  
- CD: Authenticate via service principal, deploy ADF via az deployment, sync Databricks notebooks

*Sensative information stored in Secrets and variables*
