# Welcome to Hacktitude.io challenge

>>DISCLAIMER: Please note that this project is created only for the purpose of Hacktitude.io and do NOT represent best practices of software development. The project contains purposefully placed errors, bad design practices, bad code quality and security malpractices.

## Brief about the system you are about to develop

## Setting up your environment

This section is to help your team to understand the prerequisite required in order to work on the challenges and brief about the system you are required to develop. Please read through carefully and follow the below instructions to understand how to work with the codebase of this project.

### Prerequisites

Latest stable versions of Git, Node.js and npm are required on your computer. You also must be proficient in working with the aforementioned technologies.

### install dependencies

Once you clone the project from your team's Git repository, run the following command to install dependencies.

* `npm install` to install the dependencies

### Validate if the environment is setup correctly

You can run the Sanity test file in the `tests` directory with the below command. If you have the environment correctly set up, all the tests should pass in the sanity test. If the sanity test fail, that is an indication of your environment setup issue, you must first attend to rectifying your development environment.

* `npm test -- _sanity`

### Setting up the development database

Following commands will create a SQlite database called `main.sqlite` in your root folder for development purposes. The `migrate` command will create the DB schema, and `seed` command populates the DB with some initial data. This is required for running the application.

* `npm run migrate` to create the database and establish DB schema.
* `npm run seed` to populate some data to the tables.

### Building and Running the Application

* `npm start` to start the server (without nodemon)

Now the application should run on <http://localhost:3000/>

### How to navigate in the application

* Visit 'Sign Up' and Register a new user
* Login with the new credentials of the user you just created
* Navigate the application using the main menu

### Executing the Tests

Use below commands to run the tests. When you FIRST run, all the tests except `_sanity.test` will fail.

As you complete the given challenges, respective tests will pass one by one. Once you complete all the tasks of a challenge, all tests of the respective challenge should pass.

* To run all test: `npm test`
* To run a single test file of a challenge: e.g. `npm test challenge-0`, `npm test challenge-1`

NOTE: Tests are not using the main.sqlite database. Every test creates an an isolated in-memory database.

### Improving your Developer Environment (Optional)

This step is not mandatory to work on the Hacktitude challenges, but it may improve your development experience.  

* Install a plugin for SQLite on your IDE so that you are able to explore the SQLite database.
* Install a plugin for JEST testing on your IDE. This may allow you to run a test without depending on command line.
* Install any other plugin as necessary for you to improve your developer experience.

## Solving the challenges

If your sanity test pass and you are able to run the application, now you can proceed to the challenges. All the Hacktitude challenges are documented in an own file. Please visit the links below, read carefully and get started solving them. Have fun!

* [Challenge 0](./challenge-0.md)
* [Challenge 1](./challenge-1.md)
* [Challenge 2](./challenge-2.md)
* ...

## How to get support

## References
