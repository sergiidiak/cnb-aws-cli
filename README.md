# AWS CLI Cloud Native Buildpack (CNB)

AWS CLI Buildpack provides an `aws` command during build and launch phases.

This is adoption of [Heroku AWS CLI buildpack](https://github.com/heroku/heroku-buildpack-awscli) to work with CNB (heroku & bionic stacks)

### Usage
___

Provide all necessary AWS CLI Environment variables when you build your application

```javascript

pack build my-application --buildpacks sdiak/aws-cli\
  --env "AWS_ACCESS_KEY_ID=<aws-access-key>"\
  --env "AWS_SECRET_ACCESS_KEY=<aws-secret-access-key>"\
  --env "AWS_DEFAULT_REGION=<default-aws-region>"\
```
