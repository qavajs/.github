## @qavajs

https://qavajs.github.io/

@qavajs framework is a solution that allow to significantly reduces automation project setup time due to set of predefined steps, built-in page object solution and OOB integrations with other test related stuff (like EPAM ReportPortal etc.)

### Installation from scratch
`npm init`

`npm install @qavajs/cli`

`npx qavajs install` and select modules to install. The system will generate config file based on your answers.

### Test execution
JS `npx qavajs run --config <config> --profile <profile>`

TS `npx ts-node --project tsconfig.json node_modules/@qavajs/cli/bin/qavajs.js run --config config.ts`

default config is cucumber.js 
default profile is default
