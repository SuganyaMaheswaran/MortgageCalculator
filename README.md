# Mortgage Calculator

A responsive Angular application for calculating mortgage repayment options, including standard repayment and interest-only scenarios. The app provides estimated monthly repayment, total repayment, and interest amounts based on user-entered loan details.

## Overview

This project is built with Angular 18 and uses server-side rendering (SSR) with Express. It is designed to help users quickly estimate mortgage costs before applying for a loan.

### Included features

- Mortgage amount input
- Mortgage term input
- Interest rate input
- Repayment or interest-only selection
- Monthly payment estimate
- Total repayment summary
- Interest payment summary
- Angular Material styling

## Tech stack

- Angular 18
- TypeScript
- Angular Material
- RxJS
- Express
- Angular SSR

## Prerequisites

Before running the app, ensure you have the following installed:

- Node.js 18 or later
- npm 9 or later

## Local development

1. Install dependencies:

   npm install

2. Start the development server:

   npm start

3. Open the app in your browser:

   http://localhost:4200

The Angular dev server supports hot reloading while you make changes.

## Production build

To build the application for production:

npm run build

The build output is generated into the dist/angular-app directory.

## Run the production SSR server

After building, start the SSR server with:

npm run serve:ssr:angularApp

The server listens on port 4000 by default.

To override the port:

PORT=8080 npm run serve:ssr:angularApp

## Docker

Build the Docker image:

docker build -t mortgage-calculator .

Run the container:

docker run -p 4000:4000 mortgage-calculator

The app will be available at:

http://localhost:4000

## Project structure

- src/app - application components and logic
- src/assets - static assets
- public - public static files
- server.ts - Express SSR entry point
- angular.json - Angular project configuration
- package.json - scripts and dependencies

## Notes

This app is a mortgage calculator front-end and does not persist data to a backend. The calculations are performed in the browser and the SSR server serves the generated Angular app.
