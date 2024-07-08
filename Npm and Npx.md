# Difference between Npm and Npx

### Npm

The npm stands for Node Package Manager and it is the default package manager for Node.js. It is written entirely in JavaScript, developed by  Isaac Z. Schlueter, it was initially released on January 12, 2010. The npm manages all the packages and modules for node.js and consists of command-line client npm. It gets installed into the system with the installation of node.js. The required packages and modules in the Node project are installed using npm. A package contains all the files needed for a module and modules are the JavaScript libraries that can be included in the Node project according to the requirement of the project.

**npm -v**

### Npm Commands

**npm init**: 
This command initializes a package by creating a package.json file. When you start developing a new package, npm will create a JSON file to track your dependencies and automatically update that file whenever you install or remove packages.

**npm install**: 
Install is the most commonly used npm command and you can use it in various ways. This command will install all dependencies in a package.json file if executed by itself. However, if executed as **npm install <package-name>** ,it will install a specific package from the npm registry. You can also run **npm install <package-name>** –save to install an npm package and add its dependencies to your package.json file.

**npm uninstall <package-name>**:
 This command uninstalls a specific package.

**npm update <package-name>**: 
This command updates a package to the latest version.

### Popular NPM Packages

Npm contains thousands of packages but here are five commonly used ones for you to try.

**Nodist**: This package allows you to manage your projects using npm on Windows. Nodist supports CMD, Powershell and Git bash.

**Grunt**: Grunt is a task runner that provides many plugins to automate minification, compilation and unit testing.

**Mocha**: Mocha is a testing tool that runs tests frequently, thereby allowing for flexible and accurate reporting while mapping uncaught exceptions. 

**Cheerio**: This is a fast, flexible core jQuery (database for web development).

**React**: React is a popular UI framework. It lets you build fast interfaces that scale efficiently with a focus on the essential aspects of UI design. 

### Npx

The npx stands for Node Package Execute and it comes with the npm, when you installed npm above 5.2.0 version then automatically npx will installed. It is an npm package runner that can execute any package that you want from the npm registry without even installing that package. The npx is useful during a single time use package. If you have installed npm below 5.2.0 then npx is not installed in your system.

**The primary purpose of npx is to execute packages. Without installing, it can run any package you want from the npm registry. This is particularly useful when you want to run the package only once and want to avoid installing it globally or locally.**

You can check npx is installed or not by running the following command:

**npx -v**
If npx is not installed you can install that separately by running the below command.

**npm install -g npx**

### Execution via NPM and NPX

1. **Execute package with npm:**

For executing a package using npm, we first have to install it and then you can execute it. 

Run the following command to install the required package.

**npm install package_name**

**By typing the local path**: You have to write down the local path of your package like below:

**./node_modules/.bin/your-package-name**

We can also execute it  by enlist them as a script in the package.json file and then execute them

**{
    "name": "Your app",
    "version":  "1.0.0",
    "scripts":  {
            "your-package":  "your-package-name"
     }
}**

**To run package**: After that, you can run your package by running the below command: 

**npm run your-package-name**

2. **Execute package with npx**: 

**Directly runnable**: You can execute your package without installation, to do so run the following command.

**npx your-package-name**


### Difference
1. In Npm ,If you wish to run package through npm then you have to specify that package in your package.json and install it locally.	
 In Npx a  package can be executable without installing the package. It is an npm package runner so if any packages aren’t already installed it will install them automatically.

2. To use `create-react-app` in npm the commands are `npm install create-react-app` then `create-react-app myApp` (Installation required).
 
	In npx you can create a react app without installing the package:
`npx create-react-app myApp`
This command is required in every app’s life cycle only once.


3. Npm is a tool that use to install packages.	 Npx is a tool that use to execute packages.

4. Packages used by npm are installed globally. You have   to care about pollution in the long term.	
 Packages used by npx are not installed globally. You don’t have to worry about for pollution in the long term.