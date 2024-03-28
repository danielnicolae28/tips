####################

Eslint and vite project BASIC setup

1.  npm install vite-plugin-eslint --save-dev
2.  add in vite.config.ts : 

    import eslint from 'vite-plugin-eslint';

    export default defineConfig({
       plugins: [react(),--- this part eslint() ---],
    });

3.  npm install eslint --save-dev
4.  npm install eslint-config-react-app --save-dev
5. create  .eslitrc file and add in file :
    {
     "extends": [
         "react-app"
         ]
    }

IF unassigned variables have errors you should add in :

module.exports = {
  root: true,
  env: { browser: true, es2020: true },
  extends: [
    'eslint:recommended',
    "plugin:@typescript-eslint/eslint-recommended",
        "plugin:@typescript-eslint/recommended",
    'plugin:react-hooks/recommended',
  ],
  ignorePatterns: ['dist', '.eslintrc.cjs'],
  parser: '@typescript-eslint/parser',
  plugins: ['react-refresh',"@typescript-eslint"],
  rules: {
    'react-refresh/only-export-components': [
      'warn',
      { allowConstantExport: true },
    ],
    "no-unused-vars": "off",
    "@typescript-eslint/no-unused-vars": ["warn"]
  },
}

in your .eslintrc.cjs





####################

####################

Tailwindcss with vite TSX project






####################

