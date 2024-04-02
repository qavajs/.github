## @qavajs

https://qavajs.github.io/

@qavajs framework is a solution that significantly reduces the setup time of automation projects. It provides a set of predefined steps, built-in page object solution and out of the box integrations with tools (like EPAM [ReportPortal](https://reportportal.io/), [Mobitru](https://mobitru.com/), BrowserCube,  etc.)

### Installation from scratch
`npm init @qavajs`

and select modules to install. The system will generate a config file based on your answers.

### Test execution
`npx qavajs run --config <config> --profile <profile>`

- default config is config.js or config.ts
- default profile is default
