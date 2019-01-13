# Postman - JavaScript - API Tesing Example

This is a sample implementation of API test in postman with javascript

Follow the steps below to download and run this project.

## Depedencies

Install these prerequisites to follow along with the tutorial. See free video tutorial or a full explanation of each prerequisite.

- NPM: https://nodejs.org
- Postman: https://www.getpostman.com
- Newman: https://www.npmjs.com/package/newman

## Step 1. Clone the project
`git clone https://github.com/ankurjain00/API-test-automation-postman.git`

## Step 2. Install dependencies

- Download Postman https://www.getpostman.com/downloads
- Download nodejs https://nodejs.org
```
$ npm install -g newman
$ npm install -g newman-reporter-html
```
## Step 3. Generate Postman X-API-Key
1. Hit url https://web.postman.co/integrations/services/pm_pro_api
2. Click Get API Key
3. Set API Key as X-API-Key value as collection variable

## Step 4. Run the Postman Test using Newman
`$ newman run "Postman Collections API.postman_collection.json" -e Dev.environment.json -r cli,html --reporter-html-temple templates/htmlreqres.hbs --reporter-html-export reports/my_report.html`
