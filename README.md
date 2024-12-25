The Coworking Space Service is a set of APIs that enables users to request one-time tokens and administrators to authorize access to a coworking space.

This service follows a microservice pattern and the APIs are split into distinct services that can be deployed and managed independently of one another.

4 APIs are exposed in the python application:
    1. /api/reports/daily_usage
    2. /api/reports/user_visits
    3. /readiness_check
    4. /health_check

- Created the EKS cluster
- Configured the postgress DB service
- Dokerize the application
- Setting up Continuous Integration with CodeBuild
  - Created the ECR repository to store the images
  - Created the Codebuild broject to automate teh deployment process
- Deployed the application
- Set up the cloudwatch for logging
