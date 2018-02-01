

# how-to-webpack-pc
Tools Prerequisites PC preperation for webpack module based ES6 development of html components AKA pages


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

## Yarn
After this set your installation to yarn by installing yarn
'''
npm install -g yarn
'''
### Global
https://yarnpkg.com/lang/en/docs/cli/global/

## Install webpack
'''
yarn global add webpack
'''
