# API Testing

## Project Overview

Welcome to the API Testing Project! This repository is focused on a API testing project using Postman, a powerful tool for API testing, to ensure that APIs function correctly, reliably, and securely.
To automate the execution of tests and generate detailed test reports I have used Newman, a command-line collection runner for Postman. 

I have utilized various HTTP methods, including GET, POST, PUT, and DELETE, which are fundamental for developing RESTful APIs. These methods were employed to interact with the RESTful APIs hosted at https://restful-booker.herokuapp.com/.

This readme file will guide you through the setup, usage, and best practices for this project.

## Getting Started

Before you begin using this API testing project, ensure you have the following prerequisites installed:

- **Postman**: Download and install the Postman application from [postman.com](https://www.postman.com/downloads/).

- **Node.js and NPM**: Newman is a Node.js application, so make sure you have Node.js and NPM installed. You can download them from [nodejs.org](https://nodejs.org/).

- **Newman**: Install Newman globally by running the following command:

  ```bash
  npm install -g newman

- **Report**: Install Newman Report globally by running the following command:

  ```bash
  npm install -g newman-reporter-html
	npm install -g newman-reporter-htmlextra

## Project Structure

- **collections/**: Store your Postman collections as JSON files. Collections contain a set of API requests and tests.

Here I have attached collections of APIs for the following HTTP methods: GET, POST, PUT, and DELETE, as follows:

![p1](https://github.com/rabeya19/API_Testing/assets/50509949/8ffa7550-c3db-4c61-a8ec-2003e2b5cf9c)

![p2](https://github.com/rabeya19/API_Testing/assets/50509949/5ef38e0f-5190-4196-9dc0-34be969a1fd0)

![p3](https://github.com/rabeya19/API_Testing/assets/50509949/739dbf63-29ed-496f-89d8-1846c9b13cc1)

![p4](https://github.com/rabeya19/API_Testing/assets/50509949/4cd413a7-aa04-4981-ac94-0cc7df2d86e5)

![p5](https://github.com/rabeya19/API_Testing/assets/50509949/fd689ea9-e3fb-44bd-b2fd-ab349263728d)

![p6](https://github.com/rabeya19/API_Testing/assets/50509949/8d6f09f8-dd1f-498e-a9aa-7ae4ab15f6a4)

- **environments/**: Store Postman environment files, which allow you to manage variables for different environments (e.g., development, staging, production).

Here I have attached the project environment settings:

![environment](https://github.com/rabeya19/API_Testing/assets/50509949/507f64c9-c5bb-4f9e-80cf-56b5302cf1f3)

- **reports/**: Generated test reports, such as HTML reports or JSON files, will be stored here.
To run tests using Newman, open your command line interface and navigate to the project root directory. Then, use the following command:

```bash

newman run CollectionName.json -e EnvironmentName.json -r cli,htmlextra

```

Here I have attached the generated JSON report for my project:

![newmanReport](https://github.com/rabeya19/API_Testing/assets/50509949/4aee49e6-26ac-4324-a75c-d4f20093098c)

## Feedback and Questions

If you have any questions, need clarification, or wish to provide feedback on the testing process or this README, please feel free to reach out. Open and transparent communication is essential for maintaining product quality.

