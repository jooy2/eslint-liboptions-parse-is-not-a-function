# ESLint 8.23.0 TypeError: this.libOptions.parse is not a function

- Issue: https://github.com/eslint/eslint/issues/16250

```shell
TypeError: this.libOptions.parse is not a function

TypeError: this.libOptions.parse is not a function
    at ESLint8Plugin.<anonymous> (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:139:64)
    at step (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:44:23)
    at Object.next (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:25:53)
    at C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:19:71
    at new Promise (<anonymous>)
    at __awaiter (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:15:12)
    at ESLint8Plugin.invokeESLint (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:133:16)
    at ESLint8Plugin.<anonymous> (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:120:44)
    at step (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:44:23)
    at Object.next (C:\Program Files\JetBrains\WebStorm 2020.2.2\plugins\JavaScriptLanguage\languageService\eslint\bin\eslint8-plugin.js:25:53)
Process finished with exit code -1
```

## How to reproduce
1. clone this project
2. run `npm i`
3. enable `eslint` feature in your IntelliJ Project
4. open `index.js` file in `src/server`
