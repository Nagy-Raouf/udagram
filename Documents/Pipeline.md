## pipeline
### Circle ci
The order of the run jobs:
- build
    - Setting Env Variables.
    - Install NodeJS 14.15.
    - Checkout Code.
    - Install AWS CLI - latest.
    - Configure AWS Access Key ID.
    - Setting Up Elastic Beanstalk CLI.
    - Install Front-End Dependencies
    - Install API Dependencies
    - Front-End Build
    - API Build

- Deploy
    - Setting environment
    - Setting Up Elastic Beanstalk CLI.
    - Install AWS CLI - latest.
    - Configure AWS Access Key ID.
    - checkout code
    - Deploy app
        - Deploy frontend to AWS S3.
        - Deploy backend to AWS Elastic