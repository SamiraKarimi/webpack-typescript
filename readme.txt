1. tsc --init
2. change "target": "es2016" ===>  "target": es6 
3. change "module": "commonjs" ==> "module": "es2015"
4. npm init and press enter for all of the question
5. npm install webpack webpack-cli ts-loader -D
6. npm install typescript -D ===> -D means install it as a dev dependency. We do it even tho we already have it globaly to have it locally as a dev dependency as well.
// time to work on the folder structure
1. create a "src" forlder (all of tsc file going to be there)
2. create a folder call "public" or "dist" that is all of my html, javascript, and  css file that I want to do deployment for them.
3. start adding some files on public and src

// In order to tell webpack how to compile and bundle our code we need to create webpack config file.
1. touch webpack.config.js and define an entry point for your file
2. also we have to define output base on whatever we want to have in or public folder
3. we also need to have 'absolout path' for our output. we also need rules that can check to see if our file is ts file.
the way that webpack can do for us is : 
        1. go to package.json
        2. inside of scripts -> "build": "webpack" -> it runs webpack for us, so it will go to webpack.config file and run all of that comments

know we can go to our terminal and run npm run build since we called it build;

//preview our code on the fly on our browser and also rerun
1. npm install webpack-dev-server -D
2. and then we will go to package.json to create new script to run that and name can be anything and know we have it with "npm run serve"


//for adding more ts module add resolve to the webpack.config.js

///source map is for better debugging
1.sourceMap : true;

