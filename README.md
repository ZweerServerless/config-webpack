# Zweer Serverless: Config Webpack

## Installation

This submodule must be 2 folders away from the root of the project.

You have to install it (to let npm/yarn handle its dependencies) putting this in your `package.json`:

```json
"devDependencies": {
  ...
  "config-webpack": "./config/webpack"
  ...
}
```

Finally put this in your `serverless.yml`:
```yaml
custom:
  webpack: ./config/webpack/config/serverless.js
  webpackIncludeModules:
    packagePath: ./package.json
```
