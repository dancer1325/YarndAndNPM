# Notes:
* CLI Commands -- https://docs.npmjs.com/cli/v8/commands --
  * `npm init` 
    * Start the project
  * `npm install`
    * Install / Add a dependency 
    * Example: 
      * `npm install`
        * Install all dependencies placed in package.json
      * `npm install Scope/NameOfTheDependency` -- `npm install lodash` 
        * Add 'lodash' dependency to the package.json and install it 
      * `npm install Scope/NameOfTheDependency@<version | tag | version range>` -- `npm install lodash@15`
        * Add 'lodash', version 15 dependency
    * Installation's scope
      * global
        * Example
          * `npm install -g/-global lodash`
      * local
        * Example
          * `npm install lodash`
    * Types of installation
      * development
        * Example
          * `npm install lodash -D` -- Since scope isn't specified --> it's locally --
      * normal
        * Example
          * `npm install lodash` -- Since nothing has been specified --> it's locally and normal --
  * `npm list`
    * List all the first dependencies
    * `npm list NameOfADependency`
      * Show the dependency tree of NameOfADependency 
 


