# eslint-plugin-i18n-lingui

ESLint Plugin to enforce i18n best practices.

## Installation

### Local Development

1. clone the repo in the parent directory of your project
2. Add the plugin to your project's `node_modules`:
    ```
    $ yarn add ../eslint-plugin-react-i18n --save-dev
    ```
3. In your project's `.eslintrc.js`, add

    ```js
    module.exports = {
        ...
        plugins: [
            "react-i18n"
        ],
        rules: {
            "react-i18n/no-eval-in-placeholder": 1, // warning
            "react-i18n/prefer-unicode-ellipsis": 2, // error
        }
    }
    ```

## List of supported rules

| Has Fixer | Rule                               | Description                                             |
|-----------|------------------------------------|---------------------------------------------------------|
|           | [no-eval-in-placeholder](https://github.com/OkCupid/eslint-plugin-i18n-lingui/blob/main/docs/rules/no-eval-in-placeholder.md)             | No evaluation of placeholder values in wrapped strings  |
|    ✔️      | [react-i18n/prefer-unicode-ellipsis](https://github.com/OkCupid/eslint-plugin-i18n-lingui/blob/main/docs/rules/prefer-unicode-ellipsis.md) | Detects three periods in Trans or t tag wrapped strings |
