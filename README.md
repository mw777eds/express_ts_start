## express\_ts\_start
  __  ____          ________ ______ ______ _____   _____ _____ 
 |  \/  \ \        / /____  |____  |____  |  __ \ / ____/ ____|
 | \  / |\ \  /\  / /    / /    / /    / /| |__) | |   | |     
 | |\/| | \ \/  \/ /    / /    / /    / / |  _  /| |   | |     
 | |  | |  \  /\  /    / /    / /    / /  | | \ \| |___| |____ 
 |_|  |_|   \/  \/    /_/    /_/    /_/   |_|  \_\\_____\_____|

### Project Description
General node express app starting point to be written in typescript with instructions here how to get to this point in the project.  This is for reference, training, and quick starts.


### Global Installs
Required globally installed npm packages used for development

1. [git][https://git-scm.com]
2. [node.js][https://nodejs.org/en/]
3. [npm][https://www.npmjs.com/]
4. [eslint][http://eslint.org/] *Only used as a code checker within my IDE*
5. [grunt][https://gruntjs.com/]
6. [grunt-cli][https://github.com/gruntjs/grunt-cli]
7. [yo][https://www.npmjs.com/package/yo]
8. yo generators
  1. [generator-eslint][https://www.npmjs.com/package/generator-eslint]
  2. [generator-gruntfile][https://www.npmjs.com/package/generator-gruntfile]
9. [yarn][https://yarnpkg.com/en/]

_To test what packages you have installed globally run the following command in the terminal:_`npm list -g --depth=0`

### Create the following directory structure
`README.md` is your version of this file.
`.gitkeep` are empty files used to save directory structure in git.
```
your_project/
|-- dist/
    |-- final/
        |-- .gitkeep
|-- src/
    |-- README.md
    |-- app/
        |-- .gitkeep
```

### Initialize site following these commands
_Initialization is done from the root of your project_

* **First Commit with directory structure**
  * _Make directory structure above_
  * `git init` _Create new repository for this project_
  * Create `.gitignore` _See Git Ignore area below_
* **Initializes node project, installs express, typescript, grunt, and grunt-contribs**
  * `npm init` _Create `package.json`_
  * `npm install --save express` _Install node [expressjs][https://expressjs.com/] locally._
  * `npm install --save-dev typescript` _Install [Typescript][https://www.typescriptlang.org/] locally._
  * `npm install --save-dev grunt` _Install [Grunt][https://gruntjs.com/] locally._
  * `npm install --save-dev grunt-contrib-watch` _Install [Grunt watcher][https://www.npmjs.com/package/grunt-contrib-watch] package._
  * `npm install --save-dev grunt-ts` _Install [Grunt Typescript][https://www.npmjs.com/package/grunt-ts] package_
* **Set up Configurations: tsconfig.json, Gruntfile.js, and initialize yarn**
  * `tsc --init` _Create tsconfig.json_
  * _Edit `tsconfig.json` to fit your style and needs_
  * `yo gruntfile` _Create `Gruntfile.js` with both options de-selected_
  * _Edit `Gruntfile.js` to fit your style and needs_
  * `yarn init` _Initialize yarn package tracking_
  * `eslint --init` _sets up eslint code hints for IDE_

### Git Ignore Setup
Add information to `.gitignore` to describe files and folders not included in Git.  My current set up is the following:
I got most of this from the node.gitignore [example][https://github.com/github/gitignore/blob/master/Node.gitignore]
```
# Logs
logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# Runtime data
pids
*.pid
*.seed
*.pid.lock

# Coverage directory used by tools like istanbul
coverage

# Grunt intermediate storage (http://gruntjs.com/creating-plugins#storing-task-files)
.grunt

# Bower dependency directory (https://bower.io/)
bower_components

# Dependency directories
node_modules/

# Optional eslint cache
.eslintcache

# Optional REPL history
.node_repl_history

# Output of 'npm pack'
*.tgz

# Yarn Integrity file
.yarn-integrity

# dotenv environment variables file
.env

# Mac OS
.DS_Store
```
