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
delete node_modules folder and package-lock.json, and re-install
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

# How to make an Ionic project with npx
```
npm install -g @ionic/cli
```
```
ionic start myApp tabs --type=angular --capacitor
```
startar-template: tabs, blank, sidemenu  
project type: --type=angular  
native: --capacitator, cordova  

# How to use a specific version of Ionic
https://medium.com/headerlabs-india/how-to-install-two-versions-of-ionic-on-system-d5f05c6ead38  
```
ionic start helloionic1 blank             //////////for ionic 1
ionic start helloionic2 blank --v2 --ts  ////////// for ionic 2
```
```
nvm ls-remote
```
```
nvm install v5.0.0   ///////for ionic 1
nvm install v6.4.0   ////// for ionic 2
```
```
npm -v
```
```
 For ionic 1
 cd ionic1
 nvm use
 nvm install v5.0.0
 npm install -g ionic@1.7.15 
 ionic start helloionic1 blank
 cd helloionic1
 ionic serve

For ionic 2
 cd ionic2
 nvm use
 nvm install v6.4.0
 npm install -g ionic@beta
 ionic start helloionic2 blank --v2 --ts 
 cd helloionic2
 ionic serve
```
