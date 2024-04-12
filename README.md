# BaB Online Shop

_BaB Online Shop_ is a fullstack e-commerce application build with Next.js, TypeScript and TailwindCSS.<br />
BaB stands for _Banousadhi Ayurved Bhandar_ and is an Indian traditional medicine shop for "_traditional medicines from the forest_".

## Project Configs

1. Cleanup the project first
2. Add ESLint and Prettier support to Next.js Project:

   - Install ESLint, Prettier and related plugins
     ```
       npm install --save-dev prettier eslint-config-prettier eslint-plugin-prettier
     ```
   - Add .eslintrc.json, .prettierrc files if not present already for adding configs

     ```
       eslintrc.json:
       {
         "extends": [
           "next/core-web-vitals",
           "prettier",
           "plugin:prettier/recommended"
         ],
         "plugins": ["prettier"],
         "rules": {
           "prettier/prettier": "warn"
         }
       }
     ```

     ```
       .prettierrc:
       {
          "semi": true,
          "trailingComma": "all",
          "singleQuote": false,
          "jsxSingleQuote": false,
          "tsxSingleQuote": false,
          "printWidth": 80,
          "tabWidth": 2
        }
     ```

   - For Linting & Formatting add this to your package.json file:
     ```
       "scripts": {
          "dev": "next dev",
          "build": "next build",
          "start": "next start",
          "lint": "next lint",
          "format": "prettier --write ."
       },
     ```
