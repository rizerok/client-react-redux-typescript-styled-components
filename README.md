1) Clone this repository
2) create ```.env``` like example ```example.env```
3) npm i
4) use npm scripts
```json
  {
      "build:dev": "NODE_ENV=development webpack --progress",
      "watch:dev": "NODE_ENV=development webpack-dev-server --progress",
      "build:prod": "NODE_ENV=production webpack --progress",
      "lint": "eslint -c \"./eslint/common.eslintrc.js\" \"**/**.ts*\" && stylelint \"**/**.scss\"",
      "lint:fix": "eslint \"**/**.tsx*\" --fix && stylelint \"**/**.scss\" --fix",
      "commit": "git-cz"
    }
```

`npm run build:dev` - build dev version in `/public` directory.

`npm run build:prod` - build prod version in `/public` directory.

`npm run watch:dev` - for development.

`npm run lint` - check syntax error and warring.

`npm run lint:fix` - try fix syntax error and warring.

`npm run commit` - helper for git.

