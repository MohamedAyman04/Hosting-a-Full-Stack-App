# Pipeline Process

## overview

- we specify it's version `2.1` in version
- then we do the orbs which has

```
    node: circleci/node@5.0.2
    eb: circleci/aws-elastic-beanstalk@2.0.1
    aws-cli: circleci/aws-cli@3.1.1
```

- then the jobs
- it has build and deply commands to take care of everything

## build

1. it installs `node version 16.15.1`
2. install the `front-end` dependencies
3. install the `back-end` dependencies
4. runs lint on the `front-end`
5. builds the `front-end`
6. builds the `back-end`

## deploy

1. it installs `node version 16.15.1`
2. sets up `eb (elastic beanstalk)` and `aws-cli`
3. deploys the app

## workflow

- it runs `build`
- then it runs `deploy`
