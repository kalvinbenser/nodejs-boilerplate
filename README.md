## node babel setup

```
npm install @babel/cli @babel/core @babel/node @babel/preset-env @babel/runtime --save-dev

```

#### create .babelrc file and add below code for config

```
{
  "presets": [
    "@babel/preset-env"
  ]
}

```

#### add scripts in your package.json

```
"build": "babel ./src --out-dir ./build",
"prod": "npm run build && node build/index.js",
"start": "nodemon --exec babel-node src/index.js",

```

## node prettier setup

```
 npm install prettier --save-dev

```

#### create .prettierrc file in your product root folder and add below code in your .prettierrc file

```
{
    "trailingComma": "es5",
    "tabWidth": 4,
    "semi": false,
    "singleQuote": true
  }

```

## eslint setup

```
 npm install eslint --save-dev

 npx eslint --init

```

#### add scripts npx eslint . in your package.json

```
"lint":"npx eslint ."

```

#### add .eslintignore in your project root directory.then ignore node modules,build folders

```
node_modules
build

```
