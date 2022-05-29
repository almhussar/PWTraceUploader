# PWTraceUploader

The **PWTraceUploader** is an **Azure DevOps Extension** which - as its name implies - uploads [Playwright](https://playwright.dev) test run trace files into an Azure DevOps release pipeline test results.

## Prerequisites
- There should be at least one [Publish Test Results](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/test/publish-test-results?view=azure-devops&tabs=trx%2Cyaml) task in the Azure DevOps pipeline
- [Node.js](https://nodejs.org/en/download/) must be installed on the server which is responsible for running the Playwright tests.

## Parameters
- **TargetTaskName**: The name of the Publish Test Results task which publish the results of the Playwright test runs.
- **TestResultFileDirectory**: The path of directory where the Playwright test results' xml files will be created. In general, it's the same directory which contains the Playwright tests in a default configuration.

## Known limits
- Currently it works with **TypeScript** based tests only

