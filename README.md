# Notes:
* CLI Commands -- https://docs.npmjs.com/cli/v8/commands --
  * `npm init` 
    * Start the project
  * `npm install`
    * Install / Add a dependency 
    * Example: 
      * `npm install`
        * Install all dependencies placed in package.json
      * `npm Scope/NameOfTheDependency` -- `npm lodash` 
        * Add 'lodash' dependency to the package.json and install it 
      * `npm Scope/NameOfTheDependency@<version | tag | version range>` -- `npm install lodash@15`
        * Add 'lodash', version 15 dependency
  * `npm list`
    * List all the first dependencies
    * `npm list NameOfADependency`
      * Show the dependency tree of NameOfADependency 
 


