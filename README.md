# How to make a specific version of Angular CLI  
```
npm uninstall -g @angular/cli
```
```
npm cache clean --force
```
(1st method)  
```
npm i @angular/cli@12
```
```
npx ng version
```
```
npx ng new PROJECT_NAME
```
(2nd method)  
```
npx -p @angular/cli@16 ng new PROJECT_NAME
```
```
npx ng g c components/header
```

# How to use a specific version of Node.js  
A list of Node.js that you can install
```
nvm ls-remote
```
You can also choose
```
nvm ls-remote 18
```
How to install
```
nvm install v18.13.0
```
A list of Node.js that you installed
```
nvm ls
```
Uninstall a specific version
```
nvm uninstall v14.12.0
```
Use a specific version
```
nvm use v16.16.0
```

# How to adopt to the existing projects
check if angular/cli is in devDependencies in package.json
```
npm install --save-dev @angular/cli
```
```
rm -rf node_modules package-lock.json
npm install
```
ng serve
```
npx ng serve --open
```
Or add npm scripts in package.json
```
"scripts": {
  "start": "ng serve",
  "build": "ng build",
  // other scripts
}
```
