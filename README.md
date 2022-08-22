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
  * `yarn outdated`
    * It's not working properly, since it just return the yarn version
  * `yarn upgrade`
    * Update dependency version. Example: 'yarn upgrade lodash'
  * `yarn list`
    * List all the dependencies
  * `yarn remove`
    * Remove a dependency. Example: 'yarn remove lodash'
    * Any kind of dependency can be removed
  * `yarn login`
    * Add username and email. Password is just required when you push
  * `yarn logout`
    * Remove user added previously
  * `yarn publish`
    * Publish to npm registry. By default it will be private.
      * --access privateOrPublic
  * `yarn version`
    * Get either yarn version or version package.json.
      * Options to change it
        * Manually indicating the version to use
        * --patch / --major / ...
  * `yarn link` 
    * Link to another package



