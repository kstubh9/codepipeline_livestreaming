# Livio - Livestreaming App Deployment with AWS DevOps Pipeline 

## Overview

This project demonstrates the implementation of a comprehensive CI/CD pipeline for frontend of a live streaming web app using AWS DevOps tools. The focus is on maintaining a clear separation between the development (dev) and production (prod) branches, ensuring controlled and efficient deployment workflows.

## Technologies Used

- **AWS CodeCommit:** Version control repository hosting.
- **AWS CodeBuild:** Build and compile project artifacts.
- **Amazon S3:** Artifact storage for efficient versioning.
- **AWS CodeDeploy:** Automated deployment to different environments.
- **AWS CodePipeline:** End-to-end CI/CD pipeline orchestration.
- **AWS IAM:** Role-based access control, permissions, and policy management.
- **HTML/CSS:** Front-end development for the live streaming web app.

## Project Highlights

- Branching Strategy:
  - **`prod`:** Production branch.
  - **`dev`:** Development branch.
    
- CI/CD Pipeline:
  - CodeBuild for building the project.
  - S3 for artifact storage.
  - CodeDeploy for automated deployment.
  - CodePipeline for end-to-end pipeline automation.

- Role-based Access:
  - IAM utilized for assigning permissions and policy management.

## Workflow:

1. Develop the front end using HTML/CSS.
2. Manage code in AWS CodeCommit with separate branches for development and production.
3. Utilize CodeBuild for building the project and S3 for artifact storage.
4. Automate the deployment process with CodeDeploy.
5. Implement a CI/CD pipeline using CodePipeline for end-to-end automation.
6. Utilize IAM for role-based access control and policy management.

## Collaboration and Finalization

- Separate dev and prod branches ensure controlled development and production updates.
- PRs created upon finalization in the dev branch.
- Merging into main triggers automated deployment, updating the production environment.

## Project Structure

- **`/`:** Contains the HTML and CSS code for the front-end, appspec.yml for AWS CodeDeploy and buildspec.yml for CodeBuild
- **`/scripts/`:** Contains bash scripts for installing and enabling Nginx to serve static files.
