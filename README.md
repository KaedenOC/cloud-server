# Lab 16

## Project: Cloud Server Test - AWS

## Authors: Kaeden O'Meara

## Problem Domain

Deploy a basic server to AWS Elastic Beanstalk.

## Links and Resources

- [GitHub Actions ci/cd](https://github.com/KaedenOC/cloud-server/actions)
- [GUI Deploy url](http://cloud-server-env.eba-5gmpjmym.us-west-1.elasticbeanstalk.com/)
- [CLI Deploy url](http://cloud-server-dev.us-west-1.elasticbeanstalk.com/)

## Collaborators

Reece Renninger
Tim Maupin
Ike

## Setup

*For GUI deployment*:

- Create Environment
- Application Name (can be same as others)
- Environment Name (can left be default)
- Platform - Node.js
- Platform Branch - Node.js 18 ~ Version 5.8.2 (recommended)
- Upload your code - give version name & local file, upload zip (including Json & server.js DO NOT NAME INDEX.JS)
- Single Instance (default)
- Exisiting Service Role: aws-elasticbeanstalk-service-role
- EC2 instance profile: aws-elasticbeanstalk-ec2-role
- Skip to Review, and Deploy!

*For CLI deployment*:

- `eb init` in terminal
use default names, select a region, answer No to options
- After making sure you ACP to Github, eb create
default names, select region, answer No to options
- create auto deploys but if you make changes to code base ACP to Github & then eb deploy
Routes
- `/`  Proof of life route
- `/Hello?Name=<name>` Proof of life with query

## Tests

To run tests, after running `npm i`, run the command `npm test`
