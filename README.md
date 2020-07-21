# Postman - JavaScript - API Tesing Example

This is a sample implementation of API test in postman with javascript

Follow the steps below to download and run this project.

## Dependencies

Install these prerequisites to follow.

- NPM: https://nodejs.org
- Postman: https://www.getpostman.com
- Newman: https://www.npmjs.com/package/newman

## Step 1. Install dependencies

- Download Postman https://www.getpostman.com/downloads
- Download nodejs https://nodejs.org
```
$ npm install -g newman
$ npm install -g newman-reporter-html
```
## Step 2. Generate Postman X-API-Key
1. Hit url https://web.postman.co/integrations/services/pm_pro_api
2. Click Get API Key
3. Set API Key as X-API-Key value as collection variable

## Step 3. Run the Postman Test using Newman
`$ newman run -e Dev.environment.json --reporters cli,html --reporter-html-template templates/htmlreqres.hbs --reporter-html-export reports/my_report.html "Postman Collections.json"`
