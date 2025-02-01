# Node JS

    Node JS is a runtime enviroment to run javascript files in the terminal

    Here there is no window object, but we have different objects here, like global

# Process 
        This object provides information about, and control over, the current Node.js process.

        * process.argv returns an array of the arguments passed while running the code.

# Module Exports

    Transfering Data within the same directory

        * module.exports = what you want to export

        * This exported data need to be imported using the require method. Example: 
        const someVal = require("./math")
    
        * module.export only exports one this at a time, so we can send multiple things using the export by combining them into a object.

        * We can also export by using 
            exports.var_name; (we can even give defination here too)

# importing and exporting

    We need to use the export keyword in the parent file. Example: export const a =5;

    This exported data can be imported using:
        import {what you need to import} from "filepath"

        But make sure to add type:"module" in package.json

    Transfering data within different directories

        * We need to collect the data which we need to export into index.js file in that directory

        * Then we need to pass the address of that directory in the require function (don't pass the file name)

        * The require function searches for index.js and imports that

# Node Package Manager (npm)

    * npm is the standard package manager for Node.js

    * it allows us to install packages from a large library

    * it is a command line tool

    * installing packages: npm install package_name

    * local installation: npm by defaults installs the packages locally.

    * global installation

        use npm install -g package_name (but the terminal should have admin rights)

        inorder to import these package we need to use npm link package_name

    * node_modules: This directory contains every installed dependency/packages of your project

    * package-lock.json : It records the exact version of every installed dependency, including its sub-dependencies and their versions.

    * package.json 
        The package.json contains all the information about your project, such as name, dependecies required to run, version.

        We don't need to push node_modules or package-lock.json because they can be installed using package.json file.

# Library VS Framework

    Both are prebuilt codes but library provides tools for some specific purpose but frameworks provides the overall structure.

  