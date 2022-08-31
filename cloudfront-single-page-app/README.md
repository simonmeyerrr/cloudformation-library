# CloudFront Single Page App

This CloudFormation template helps to deploy single page application (React, Vue, Angular, ...) on AWS.

/!\ Use this template only in `us-east-1`.

## Resources

### CloudFront + S3 Hosting

A CloudFront Distribution linked to an S3 Bucket which contains the build of the single page app.

It also resource to secure this communication with strict S3 Bucket Policy and CloudFront Origin Access Identity.

### Password Protection Function (optional)

A CloudFront Function which blocks public access with customizable username and password.

### Github Deployment Role (optional)

An IAM Role which makes possible to deploy easily from Github Action using OpenId Identity Provider.

## TODO

- Add CloudFront custom domain (with certificate) configuration
- Add CloudFront logging settings configuration
- Add CloudFront WebACL settings configuration
