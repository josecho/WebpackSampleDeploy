# WebpackSampleDeploy

 Webpack-Based Deployment for Static Sites
 
 Create repository WebPackSampleDeploy
 
 In local machine:
 git init
 git add .
 git commit -m "initial commit"
 git remote add origin https://github.com/josecho/WebpackSampleDeploy.git
 git checkout -b gh-pages
 git subtree push --prefix dist origin gh-pages
 
 OR
 
 PACKAGE.JSON
 ...
 "scripts": {
    "clean": "rimraf dist",
    "build": "NODE_ENV=production npm run clean && webpack -p",
    "serve": "webpack-dev-server"
    "deploy": "npm run build && git subtree push --prefix dist origin gh-pages"
  },
 ...
 
 
 RESULT:
  https://josecho.github.io/WebpackSampleDeploy/#/
 
