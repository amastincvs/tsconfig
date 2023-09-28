# tsconfig

> Modular configuration for TypeScript

This package supplies a number of TypeScript configurations to the entire monorepo.
Configuration files are scoped by concern, and extend a common base configuration.
By using a predefined configuration across all projects of the same concern, it ensures that those projects will behave consistently and that best practices are followed.

## Extending the base configuration

First, create a new `.json` file in this directory.
The name of the file should be the name of the configuration you want to create.
For example, if you want to create a configuration for a Node.js project, you would create a file called `node.json`.

Next, add the following to the file:

```json
{
  "$schema": "https://json.schemastore.org/tsconfig",
  "display": "YOUR_DISPLAY_NAME_HERE",
  "extends": "./base.json"
}
```

Finally, add any additional configuration options you want to add to the file.

For more information on `tsconfig.json`, see the [docs](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html).
