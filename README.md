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
  * `npm outdated`
    * Based on the package.json's placeholders ⟶ it gives to us the dependencies which can be updated
  * `npm update [<PackageName>] [--dev]`
    * Update a PackageName
      * Just the one's specified at top-level in packages.json, not inherited one's
      * to the 'wanted' version
        * If you want to update to a specific version ⟶ use `npm install ...@SpecifiedVersion` 
    * Stage / type of installation can be specified
    * Examples
      * `npm update`
        * Update all packages to 'wanted' version specified in `npm outdated`
      * `npm update react`
        * Update react dependency to 'wanted' version specified in `npm outdated` 
  * `npm uninstall [Scope / NameOfTheDependency] [Options]`
    * [Options]
      * If it's not indicated ⟶
        * dependency will be deleted in 'node_modules'
        * package.json will be updated
      * '--no-save'
        * dependency will be deleted in 'node_modules'
        * package.json will ⚠️  NOT ⚠️ be updated
        * uses
          * testing
  * `npm adduser [--registr=url][--scope=ScopeOfThePackage][--always-auth]`
    * Add a user in the npm's registry used in order to identify us
  * `npm login` 
    * Identify us in the npm's registry
  * `npm version [major | minor | patch | premajor | preminor | prepatch | prerelease | <newVersion>]`
    * Increase the package's version
    * Any type of convention versioning can be used:
        * SemVer
        * ComVer
        * ...
    * Example
        * `npm version patch`  --> Automatically increase the patch in the package.json
  * `npm publish [Options]`
    * 'private' attribute in 'package.json'
      * if it's false / not specified the attribute ⟶ we can publish it
      * if it's true ⟶ we can ⚠️  not publish it ⚠️
    * [Options]
      * If folder isn't specified ⟶ current folder
      * tarball
        * indicate if it's a folder in a .tar extension
      * tag
        * version to specify
      * By default, it will be published in a private organization
        * premium option
      * '--access public'
        * publish it publicly
  * `npm link`
    * Create symbolic links between packages
  * Shortcuts
    * Unnecessary to type "run"
        * Example: `npm test` === `npm run test`
    * Use just the first letter
        * Example: `npm t` === `npm run test`

