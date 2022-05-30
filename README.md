# Udagram
 The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

## EB link
- http://Udagram-env.eba-chmbcx7d.us-east-1.elasticbeanstalk.com
## S3 link
- http://myrandombucket123.s3-website-us-east-1.amazonaws.com

## Infrastructure description
```
Udagram
- node.js use for backend Elastic Beanstalk for hostings it
- Angular use for frontend S3 for hostings it
- A RDS database running Postgres
- USE MVC 

```
## Getting Started

1. Clone this repo locally into the location of your choice.
1. Move the content of the udagram folder at the root of the repository as this will become the main content of the project.
1. Open a terminal and navigate to the root of the repo
1. follow the instructions in the installation step

### App dependencies

```
- Node v14.15.1 (LTS) or more recent. 

- npm 6.14.8 (LTS) or more recent

- AWS CLI v2

- A RDS database running Postgres.

- Elastic Beanstalk for hostings the server

- A S3 bucket for hostings frontend

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework
  
## Pipeline process
 1. backend install
 1. frontend install
 1. backend build
 1. frontend build
 1. frontend test
 1. backend deploy
 1. frontend deploy
  
## License

[License](LICENSE.txt)
