1. `.prettierrc`
```
{
  "semi": false,
  "singleQuote": true,
  "tabWidth": 2,
  "printWidth": 180
}
```

2. `.eslintrc`
```
{
  "root": true,
  "plugins": ["@typescript-eslint", "unused-imports", "prettier"],
  "extends": ["eslint:recommended", "plugin:@typescript-eslint/recommended"],
  "parser": "@typescript-eslint/parser",
  "rules": {
    "prettier/prettier": [
      "error",
      {
        "endOfLine": "auto"
      }
    ],
    "no-unused-vars": "off",
    "unused-imports/no-unused-imports": "error",
    "unused-imports/no-unused-vars": [
      "warn",
      {
        "vars": "all",
        "varsIgnorePattern": "^_",
        "args": "after-used",
        "argsIgnorePattern": "^_"
      }
    ]
  },
  "env": { "node": true, "browser": true }
}
```

3. run code
```
npm install @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint eslint-config-prettier eslint-plugin-prettier eslint-plugin-unused-imports -D
```
or
```
yarn add @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint eslint-config-prettier eslint-plugin-prettier eslint-plugin-unused-imports -D
```
