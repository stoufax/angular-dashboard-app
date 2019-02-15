# Angular Core

We are going to use the Angular CLI and NRWL Extensions extensively to streamline development and free us up to focus on core concepts.

Follow the steps below to get started!

## The Stack

### NRWL Workspace
A NRWL workspace contains one or all of you Angular projects and libraries. It creates a monorepo for your applications domains. Nx helps add extra layer of tooling that can help manage your enterprise applications. 

External Video Reference: [Angular in a Microservices world](https://www.youtube.com/watch?v=d04U7SjORTI)

### Angular Material
Angular Material is a UI library for Angular that gives you access to a modern material UI that works across web, mobile, and desktop applications with minimal custom CSS and setup.

### JSON Server
Creates a quick and simple way to mock out a backend REST service. We can then deliver some mocked out data in JSON format to make sure everything is working as expected once our real backend is connected.

## Getting Started

An Nx workspace is an Angular CLI project that has been enhanced to be enterprise ready. Being an Angular CLI project means it will be handy to have the Angular CLI installed globally, which can be done via npm or yarn as well.

```
npm install -g @angular/cli
```

> Note: If you do not have the Angular CLI installed globally you may not be able to use ng from the terminal to run CLI commands within the project. But the package.json file comes with npm scripts to run ng commands, so you can run npm start to ng serve and you can run npm run ng <command> to run any of the ng commands.

After you have installed the Angular CLI, install `@nrwl/schematics`.

```
npm install -g @nrwl/schematics
```

After installing it you can create a new Nx workspace by running:

```
create-nx-workspace angular-core-app
```

The next step is to generate an app in your workspace. Do so by running:

```
ng generate app dashboard
```

You'll then be prompted to answer a few setup questions. Run the following for each question:

` In which directory should the application be generated? `   apps

` Would you like to add Angular routing?`  yes

` Which Unit Test Runner would you like to use for the application? `  Karma

` Which E2E Test Runner would you like to use for the application? `  Protractor


Lastly, please install the npm dependencies by running:
```
npm install
```
You are good to go!