# Global (Typescript) Eslint Config

## Why?
- Eslint can't @#%@#% find the typescript eslint plugin if installed globally
- The typescript-eslint bug reporting process is a nightmare
- I don't want to put a node_modules in my home folder

## Fix for eslint error
```
Oops! Something went wrong! :(

ESLint: 8.2.0

ESLint couldn't find the plugin "@typescript-eslint/eslint-plugin".
```

# How

Clone this project into some folder and edit `.eslintrc.json` to taste.

```shell
# install eslint globally
$  npm install -g eslint
# install eslint typescript plugins from this project
$  npm install
```
Edit vscode settings.json

```javascript
  "eslint.options": {
    "overrideConfigFile" : "<location-of-global-eslint-project>/.eslintrc.json"
  }
```


