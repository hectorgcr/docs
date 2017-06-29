// Copyright (c) YugaByte, Inc.

# README #

YugaByte Product Documentation

### What is this repository for? ###


Our docs are based on the Hugo framework and are using the Material Docs theme

** Hugo framework: http://gohugo.io/overview/introduction/

** Material Docs theme: http://themes.gohugo.io/material-docs/

** Example of Material docs theme: http://themes.gohugo.io/theme/material-docs/


### How do I get set up? ###

## Install Hugo ##
```
brew update
brew install hugo
brew install npm
```

## To run locally on your Mac ## 
```
npm start
```

## To publish to S3 ##
Caution: This would publish the docs to our website which is used by customers
```
npm run publish
```

The last command above starts high performance web server that continuously watches the entire docs directory. Go to [http://localhost:1313/](http://localhost:1313/)to see the docs.

Simply running "hugo" will create a directory called public that has all the html content necessary to deploy to production behind an existing web server.

Detailed installation instructions: http://gohugo.io/overview/installing/
Detailed usage instructions: http://gohugo.io/overview/usage/