# ESLint Validation

Example of a simple project that showcase a kind of issue that ESLint is expected to report.

## Configurtion file
It is expected the tool to use the *.eslintrc* on the root of the project when running:

```
  "plugins": [
    "react"
  ],
  "rules": {
    "quotes": [2, "double"]
  }
```

In this case, I depend on the *react plugin* and the rule for the quoting style of my code should be double quotes i.e **strings with single quotes must be warned by ESLint**.

## Run the tool on Linux
 * Install ESLint
    > npm install -g eslint
 * Install necessary plugins, in this case, only needs react
    > npm install -g eslint-plugin-react
 * Run the tool on the root of the repository
    > eslint .

## Expected results
The tool should return an error on line 4 of *example.js* stating that "Strings must use doublequote"
