# tailwind-vue-template
A template project with vuejs, vite and tailwind.

## package usage
* vuejs v3
* tailwind
* postcss
* vue-router (option, if you want to add routing system)

**The following process uses yarn, you can use your favorite like npm or pnpm**

## creating project
Create the project using. You can create the project using vite or vue.
```bash
# using vite
npm init vite <project_name>
# using vue
npm init vue@latest
```
Both of the above process will give you an interactive cli to set up your project.

## installing packages
After project has been created install all the dependencies.
```bash
# install initial packages
yarn
# install the tailwind and other necessary packages
yarn add --dev tailwindcss postcss autoprefixer
```

## create config files
After you have installed the above packages we then generate postcss.config.cjs and tailwind.config.js. We can do this using the following command.
```bash
# 
yarn tailwindcss init -p
```
After the files have been created we can configure them. I have created a simple configuration.
Adding only content and purge feature.

## setup css
Create index.css file in assets and add following code;
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
Import this file in main.js | app.js .

## Setup vue-router
1. create pages directory which will include all the pages.
1. create router/index.js and 

**Resources**

* [https://tailwindcss.com/docs/guides/vite](https://tailwindcss.com/docs/guides/vite)
