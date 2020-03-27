# aws-upload-utility
Simple boilerplate node utility to deploy files to an Amazon s3 bucket

## Getting Started

- Install the `aws-sdk` and `dotenv` packages (npm install --save-dev aws-sdk dotenv)
- Configure local and s3 routes for your project in `variables.env`
- Run `node s3-upload` or use npm scripts in `package.json` and deploy files to the s3 server

## Quick notes

Because s3 stores files as an object key for a bucket you can declare a "path" in the variables.env that will map your file to. This path will be created on the first run of this script and will allow you to simply overwrite the file on each run of the script. The configuration automatically sets the files to be public so everything happens all at once without need for the AWS GUI or a file upload utility.

If you need help getting your s3 credentials, view the following guide:
https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/getting-your-credentials.html