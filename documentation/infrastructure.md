# The Infrastructure

- there is a `front-end app` that runs and there is also the `back-end`
- the `back-end` has `databse and api`
- the `front-end` then can connect to this `api` to make changes in the `databse`
- the database used is `aws rds`
- the `back-end` connects to it via url
- the server used is `aws elastic beanstalk`
- and the `back-end` also connects to it via url
- when the code is pushed to github
- circleci detects it and run scripts to build and deploy the application
- so at the end everything is deployed and updated on the `aws services`
