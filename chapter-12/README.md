# Chapter 12
This directory contains useful code snippets for the Automation Testing with Cypress Book chapter 12;

We have bootstrapped our tests with the [Cypress realworld application](https://github.com/cypress-io/cypress-realworld-app) project which is a simple financial application
that is meant to help Cypress users better understand how to test Cypress applications. The application is located in the root location in the directory `cypress-realworld-app`. 

To simplify execution of the application, we will only have three commands that will be used to run our test application. One command is to run to install the dependencies, the other to run the application, while the last command's purpose will be to reset the application as it uses a json database which needs resetting if at all any 
changes were made to the database in the process.

## Application Summary
The Application is a React Typescript application with the backend built with express Js and the database low-db.

## 1. Installing our Application dependencies

This command will install our test application dependencies and start our application (both the API and the frontend)

```
npm run cypress-init

```

## 2. Running the application

This command will run our test application and start both the frontend and backend (API) and seed our low-db data. 

```
npm run cypress-app

```

## 3. Resetting the application

This command will reset our low-db database to the original state without any additions that may have been made during the process of interaction with our application. 

```
npm run cypress-app-reset

```

### Application test usernames

Katharina_Bernie 
Tavares_Barrows
Allie2
Giovanna74

All usernames have a password of `s3cret`



## Executing Tests by folder
To execute tests in this chapter one needs to get into the chapter folder and run the tests from the test folder itself as every folder is a module on its own. 

```
$ cd chapter-12
```

### Installing project dependencies for Cypress tests
```
$ npm install

or 

$ npm ci

```

### Running all Cypress Tests
```
$ npm run cypress:run
```

### Adding Percy Token (Unix)
```
export PERCY_TOKEN=YOUR_TOKEN_HERE
```

### Adding Percy Token (Windows)
```
set PERCY_TOKEN=YOUR_TOKEN_HERE
```
### Adding Applitools Token (Unix)
```
export APPLITOOLS_API_KEY=YOUR_API_KEY_HERE
```

### Adding Applitools Token (Windows)
```
set APPLITOOLS_API_KEY=YOUR_API_KEY_HERE
```