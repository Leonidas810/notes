## **How to Use package.json, the Core of any Node.js Project or npm Package**

The *package.json* file is the center of any Node.js project or [[NPM]] package. It stores information about your project. It consists of a single JSON object where information is stored in key-value pairs. There area only two required fields; name and version. but it's good practice to provide additional information

You can create the *package.json* file from the terminal using the npm init command. This will run a guided setup. Using npm init with the *"-y"* flag will generate the file without having it ask any questions, "npm init -y"

If you look at the file tree of your project, you will find the *package.json* file on the top level of the tree. This is the file that you will be improving in the next couple of challenges

One of the most common pieces of information in this file is the author field. It specifies who created the project, and can consist of a string or and object with contact or other details. An object is recommended for bigger proejcts, but a simple string like the following example will do for this project

```
"author":"Jane Doe",
```

## **Add a Description to your package.json**

The next part of a good package.json file is the *description* field; where a short. but informative description about your project belongs

If some day you plan to publish a package to npm, this is the string that should sell your idea to the user when they decide whether to install your package or not. However, that's not the only use case for the description, it's a great way to summarize what a project does. It's just as important in any Node.js project to help other developers, future maintainers or even your future self understand the project quickly.

Regardless of what you plan for your project, a description is definitely recommended. Here's an example:

```
"description": "A project that does something awesome"
```

## **Add keywords to Your package.json**

The *keywords* field is where you can describe your project using related keywords. Here's an example:

```
"keywords":["descriptive","related","words"]
```

As you can see, this field is structured as an array of double-quoted strings.

## **Add a License to Your package.json**

Some common licenses for open source projects include "MIT" and "BSD". License information is not required, and copyright laws in most countries will give you ownership of what you create by default. However, it's always a good practice to explicitly state what users can and can't do.
Here's an example of the license field:

```
"license":"MIT"
```

## **Add a Version to your package.json**

A "version" is one of the required fields of your package.json file. This field describes the current versions of your project. Here's an example:

```
"version":"1.2.0"
```

## **Expand your project with External Package from nms**

One of the biggest reasons to use package manager, is their powerful dependecy management. Instead of manually having to make sure that you get all dependencies whenever you set up a project on a new computer, [[NPM]] automatically installs everything for you. But how can [[NPM]] know exactly what your project needs? Meet the "dependencies" section of your package.json file

In this section, packages your project requires are stored using the following format:

```
"depencencies":{
	"package-name":"version",
	"express":"4.14.0"
}
```

## **Manage npm Dependencies By Understanding Semantic Versioning**

Versions of the [[NPM]] packages in the dependencies section of your package.json file follow what's called *Semantic Versioning (SemVer)*, an industry standard for sofware versioning aiming to make it easier to manage dependencies. Libraries, frameworks or other tools published on [[NPM]] should use SemVer in order to clearly communicate what kind of changes projects can expect if they update

Knowing SemVer can be useful when you develop sofware that use external dependencies (which you almost always do), One day, your understanding of these numbers will save you from accidentally introducing breaking changes to your project without understanding why things that worked yesterday suddenly don't work today. This is how Semantic Versioning works according to the official website:

```
"package" : "MAJOR.MINOR.PATCH"
```

- The *MAJOR* version should increment when you make incompatible API changes. 
- The *MINOR* version should increment when you add functionality in a backwards-compatible manner. 
- The PATCH versions should increment when you make backwards-compatible bug fixes. 

This means that PATCHes area bug fixes and MINORs add new features but neither of them break what worked before. Finally, MAJORs add changes that won't work with earlier versions

## **Use the Tilde-Character to Always Use the Latest Patch Version of Dependency**

In the last challenge, you told npm to only include a specific version of package. That's a useful way to freeze your dependencies if you need to make sure that different part of your project stay compatible with each other. But in most use cases, you don't want to miss bug fixes since they often include important security patches and (hopefully) don't break things in doing so.

To allow an npm dependency to update to the latest PATCH version, you can prefix the dependency's versions with the tilde (~) character. Here's an example of how to allow updates to any "1.3.x" versions.

```
"package" : "~1.3.8"
```

## **Use the Caret-Character to Use the Latest Minor Version of Dependency**

Similar to how the tilde we learned about in the last challenge allows npm to install the latest PATCH for a dependency, the caret (^) allows npm install future updates as well. The difference is that the carret will allow both MINOR updates and PATCHes.

```
package:"^1.3.8"
```
This would allow updates to any 1.x.x versions of the package.

## **Remove a Package from your Dependencies**

You have now tested a few ways you can manage dependencies of your project by using the package.json's dependencies section. You have also included external packages by adding them to the file and even told [[NPM]] what types of versions you want, by using special characters such as the tilde or the caret.

But what if you want to remove an external package that you no longer need? You might alredy have guessed it. just remove the corresponding key-value pair for that package from your dependencies.

This same method applies to removing other fields in your package.json as well.