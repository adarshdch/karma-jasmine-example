# karma-jasmine-phantomjs-example

Example Usage of Karma with Jasmine, PhantomJs

*Run below command from the project directory to run the tests*

* This sample application uses PhantomJS and Chrome browsers. You can add more if you want.
* It uses the jasmine example classes Player and Song for showcasing the demo.

```npm test```


## Steps followed to create this sample project

* Create a folder named "karma-jasmine-phantomjs-example".
* Navigate to this folder in command prompt.
* Install karma globally to be able to run karma command globally.
```
npm i -g karma
```
* Initialize npm package.json file by running
```
npm init
```
* Accept the default values for npm init.
* package.json file would be generated.
* Install the required dev dependencies.
```
npm i --save-dev karma jasmine jasmine-core karma-chrome-launcher karma-jasmine karma-phantomjs-launcher phantomjs phantomjs-prebuilt
```
* Initialize karma configuration file by running command.
```
karma init
```
* Accept default values for karma.
* karma.conf.js file would be generated.
* Create two folders "src" and "tests" which contains source js files and test js files respectively.
* Create source and test js files using jasmine. You can copy these files from https://github.com/jasmine/jasmine/releases as well.
* Update karma.conf.js file to configure it to include source and test js files.
```
// list of files / patterns to load in the browser
files: [
  'src/**/*.js',
  'tests/**/*.js'
],
```
* Modify package.json file configure npm test command
```
"scripts": {
  "test": "karma start"
},
```
* Run tets by running command
```
npm test
```
* You should be able to see that all test cases are passing in console

#### Enjoy playing with jasmine and karma by adding or modifying the code
