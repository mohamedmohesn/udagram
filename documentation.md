# Infrastructure description

it use `Model–view–controller (MVC)` is a software design pattern commonly used for developing user interfaces that divide the related program logic into three interconnected elements

## backend

Udagram use `node.js - Javascript Runtime ` and `Express - Javascript API Framework` use for backend and it written in `TypeScript`, it use `Elastic Beanstalk` for hosting the backend .

`Node.js` is a JavaScript runtime built on Chrome's V8 JavaScript engine.

`AWS Elastic Beanstalk` is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and IIS. 

`Express` is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

`TypeScript` is a strongly typed programming language that builds on JavaScript, giving you better tooling at any scale. 

### deploy

Follow these steps to check the health of an elastic beanstalk application

1. Start by connecting the EB CLI to the environment with `eb use Udagram-env`.
2. Check the health of the environment with the `eb health`. This will bring up a table with different information about the servers running your application.
3. If you see that the health is not indicating an "OK" status, use the `eb logs` command. This will print out the logs to your terminal. You can inspect them to look for failures.

## frontend

Udagram use `Angular - Single Page Application Framework ` use for frontend and it written in `TypeScript`, it use `Amazon S3` for hosting the frontend. 

`Angular` is an application design framework and development platform for creating efficient and sophisticated single-page apps.

`TypeScript` is a strongly typed programming language that builds on JavaScript, giving you better tooling at any scale. 

`Amazon Simple Storage Service (Amazon S3)` is an object storage service offering industry-leading scalability, data availability, security, and performance.

### deploy

to deploy Amazon S3 use `npm run frontend:deploy` to upload on it

## database

Udagram use `Postgres - object-relational database system` use for database, it use `RDS` for hosting the database. 

`PostgreSQL` is a powerful, open source object-relational database system with over 30 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance.

`Amazon Relational Database Service (RDS)` is a collection of managed services that makes it simple to set up, operate, and scale databases in the cloud

# App dependencies
## backend
```
- `Node v14.15.1 (LTS) or more recent` is JavaScript runtime built
- `npm 6.14.8 (LTS) or more recent` is Open source developers from every continent use npm to share and borrow packages
- `AWS CLI v2` is a unified tool to manage your AWS services. 
- `jsonwebtoken 8.5.1` is a compact, URL-safe means of representing claims to be transferred between two parties.
- `Elastic Beanstalk` is an easy-to-use service for deploying and scaling web applications and services
- `bcrypt 5.0.1` is A library to help you hash passwords.
- `dotenv` is a zero-dependency module that loads environment variables from a .env file into process.env

```
## frontend
```
- `Angular` is an application design framework and development platform for creating efficient and sophisticated single-page apps
- `Amazon S3` is an object storage service offering industry-leading scalability, data availability, security, and performance.
- `Jasmine Framework` is s a command line interface and supporting code for running Jasmine specs under Node for Unit tests
- `Protractor` is an end-to-end test framework for Angular and AngularJS applications for e2e tests 
- `karma` is A simple tool that allows you to execute JavaScript code in multiple real browsers

```
## database
```
- `PostgreSQL` is a powerful, open source object-relational database system 
- `RDS` is a collection of managed services that makes it simple to set up, operate, and scale databases in the cloud

```

# Pipeline process

 1. `environment is set up` this step set up node.js and npm and aws cli 
 2. `backend install` this step install packages for backend `npm run backend:install`
 3. `frontend install` this step install packages for frontend `npm run frontend:install`
 4. `backend build` this step build the backend `npm run backend:build`
 5. `frontend build` this step build the frontend `npm run frontend:build`
 6. `backend test` this step test the backend `npm run backend:test`
 7. `frontend test` this step test the frontend `npm run frontend:test`
 8. `frontend e2e` this step test the frontend `npm run frontend:e2e`
 9. `frontend deploy` this step deploy the frontend `npm run frontend:deploy`