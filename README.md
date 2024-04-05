How to make a specific version of Angular CLI  
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
