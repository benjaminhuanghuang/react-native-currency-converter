## Eslint
- https://learn.handlebarlabs.com/courses/175915/lectures/2643145

- Install
```
 npm install -g eslint
 ```
- Create eslint config
```  
  run eslint --init
```
  Select "Use a popular style guide"
  Select "Airbnb"
  Do you use React? y
  What format do you want your config file to be in? JSON
- Add to .eslintrc.json
```
{
  "extends": "airbnb", // EXISTING
  "parser": "babel-eslint",
  "env": {
    "browser": true
  },
  "plugins": [
    "react"
  ],
  "rules": {
    "react/jsx-filename-extension": [
      2,
      {
        "extensions": [
          ".js",
          ".jsx"
        ]
      }
    ],
    "react/forbid-prop-types": [
      0
    ],
    "react/require-default-props": [
      0
    ],
    "global-require": [
      0
    ]
  }
}
```
- Add npm scripts
```
// 
"scripts": {
  // ...
  "lint": "eslint app/",
  "lint:fix": "eslint app/ --fix"
},
```
- Update VSCode settings
```
{
  "prettier.eslintIntegration": true,
  "editor.formatOnSave": true
}
```