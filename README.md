




# how-to-webpack-pc
Tools Prerequisites PC preperation for webpack module based ES6 development of html components AKA pages

## Windows 10 and Powershell 5

## Install Node.JS Current

Node.JS can be installed from https://nodejs.org/en/

## Change Path for Node

To change the "global" location for all users to a more appropriate shared global location %ALLUSERSPROFILE%\(npm|npm-cache) (do this as an administrator):
create an [NODE_INSTALL_PATH]\etc\ directory 
this is needed before you try npm config --global ... actions
create the global (admin) location(s) for npm modules 
C:\ProgramData\npm-cache - npm modules will go here
C:\ProgramData\npm - binary scripts for globally installed modules will go here
C:\ProgramData\npm\node_modules - globally installed modules will go here
set the permissions appropriately 
administrators: modify
authenticated users: read/execute
Set global configuration settings (Administrator Command Prompt) 
npm config --global set prefix "C:\ProgramData\npm"
npm config --global set cache "C:\ProgramData\npm-cache"
Add C:\ProgramData\npm to your System's Path environment variable such that it is first in path

## Where npm
where npm should display


## set global cache folder
To change the "global" location for all users to a more appropriate shared global location %ALLUSERSPROFILE%\(npm|npm-cache) (do this as an administrator):

create an [NODE_INSTALL_PATH]\etc\ directory
this is needed before you try npm config --global ... actions
create the global (admin) location(s) for npm modules
- npm modules will go here
```
mkdir C:\ProgramData\npm-cache 
```
- binary scripts for globally installed modules will go here
```
C:\ProgramData\npm 
```
- globally installed modules will go here
```
C:\ProgramData\npm\node_modules 
```
set the permissions appropriately
administrators: modify
authenticated users: read/execute
Set global configuration settings (Administrator Command Prompt)
```
npm config --global set prefix "C:\ProgramData\npm"
npm config --global set cache "C:\ProgramData\npm-cache"
```
Add C:\ProgramData\npm to your System's Path environment variable

## Yarn
After this set your installation to yarn by installing yarn
```
npm install -g yarn
```
### Global
https://yarnpkg.com/lang/en/docs/cli/global/

### install angular-cli and set yarn
```
yarn global add @angular/cli
```

```
ng set --global packageManager=yarn
```

## typescript and babeljs - the time-travel machines
Both maybe needed. However, use yarn always to avoid features that are not needed when you go through the time travel machine and found the side effects of including features that you don't want to see in the present time 

## Install webpack, gulpjs, commonjs, jspm
```
yarn global add webpack
yarn global add gulp
yarn global add commonjs
yarn global add jspm
```

### List of npm commands for update and check package versions
``` batch
npm view @babel/core versions
npm update
```


https://webpack.js.org/guides/getting-started/

## Visual Studio Code
Install Visual Studio Code from https://code.visualstudio.com/

### VSCode VueJs emmmet
https://docs.emmet.io/cheat-sheet/
https://medium.com/@BjornKrols/integrating-and-customising-bootstrap-4-in-vue-js-cbc29ba7688e
https://github.com/JayDevOps/make-bootstrap-sexy-again

### VSCOde VueJS Universal - static pages
https://nuxtjs.org/
https://ssr.vuejs.org/en/universal.html
https://vuejs.org/v2/guide/ssr.html

## TypeScript configurations
```
yarn global add @types/jasmine
yarn global add jasmine
```
yarn add @types/jasmine --dev
yarn add @jasmine --dev
```
in tsconfig.json of the project update

```
"types": ["jasmine"]
```
