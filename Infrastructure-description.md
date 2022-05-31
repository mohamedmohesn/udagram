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
