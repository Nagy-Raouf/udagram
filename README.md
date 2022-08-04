# Udagram

- [Udagram](#udagram)
  - [Description](#description) 
  - [Project Setup](#project-setup)
    - [Environment Variables](#environment-variables)
    - [AWS Cloud](#aws-cloud)
    - [Scripts](#scripts)
    

## Description
This project is part of Udacity nanodegree Program.
The code is provided by Udacity to be hosted into AWS with Pipeline using CircleCI.
The project is build using angular framework and Nodejs (express).

## project setup
### Environment Variables

| Name                  |                         Value                         |
| --------------------- | :---------------------------------------------------: |
| PORT                  |                          8080                         |
| POSTGRES_HOST         |                         RDS URL                       |
| POSTGRES_DB           |                       database name                   |
| POSTGRES_USERNAME     |                   username in RDS                     |
| POSTGRES_PASSWORD     |                   password in RDS                     |
| POSTGRES_PORT         |       port used in RDS (postgres default port 5432)   |
| AWS_REGION            |                   region used in AWS                  |
| AWS_ACCESS_KEY_ID     |                 AWS Access key ID                     |
| AWS_SECRET_ACCESS_KEY |              Your AWS secret Access key               |
| AWS_S3_ENDPOINT       |             The url of the S3 hosted app.             |
| AWS_REGION            |  The AWS region you used to provision RDS, S3 and EB  |
| AWS_PROFILE           |                   Your AWS profile                    |
| AWS_BUCKET            | The name of the S3 bucket used to host the front end  |
| JWT_SECRET            |  JWT token secret, set to any value               |
| URL                   | Your backend URL, found after creating EB Environment |

### AWS Cloud

- RDS DB-Host: udagramdb-1.ckvvkwcin0gb.us-east-1.rds.amazonaws.com
- RDS DB-Port: 5432
- RDS DB-name: udagramdb-1

- Frontend URL: http://my-udagram12356-bucket.s3-website-us-east-1.amazonaws.com

- Backend URL: http://udagram-api-dev.eba-fcx5rcrf.us-east-1.elasticbeanstalk.com

### Scripts
In the root directory of the project:
- `frontend:install`: install frontend dependencies.
- `frontend:start`: start frontend
- `frontend:build`: build frontend.
- `frontend:test`: test frontend
- `frontend:e2e`: end to end testing
- `frontend:lint`: lint frontend
- `frontend:deploy`: deploy the project to S3 (uses deploy.sh script).
- `api:install`: install api dependencies.
- `api:build`: build api and zip its content
- `api:start`: start api
- `api:deploy`: deploy api on EB (uses deploy.sh script).
- `deploy`: delpoy both the frontend and backend