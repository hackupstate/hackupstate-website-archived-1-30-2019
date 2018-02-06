# Hack Upstate Website - AWS S3 Bucket Instructions

Install AWS CLI (Command Line Interface) [here](https://docs.aws.amazon.com/cli/latest/userguide/installing.html)

Create a New Access Key (if you haven't already) by going [here](https://console.aws.amazon.com/iam/home?#/security_credential).

Open a new terminal and run 

`aws configure`

You'll be prompted to enter your keys.

Repo is found [here](https://s3.console.aws.amazon.com/s3/buckets/hackupstate.com/?region=us-west-2&tab=overview#).

## Cloning repo on your machine

`aws s3 sync s3://hackupstate.com . --exclude 'archive-2-5-2018/*'`

## Pushing changes up

You can enter individual file names or to snyc everything:

`aws s3 sync . s3://hackupstate.com --exclude 'node_modules/*' --exclude '.git/*' --acl public-read`