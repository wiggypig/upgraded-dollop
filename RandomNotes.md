#Random Notes

##command CLI to find app using port 8080
``` netstat -ano | findstr 8080 ```

# Password Manager
Bitwarden 

# Maven Phases
Although hardly a comprehensive list, these are the most common default lifecycle phases executed.

validate: validate the project is correct and all necessary information is available
compile: compile the source code of the project
test: test the compiled source code using a suitable unit testing framework. These tests should not require the code be packaged or deployed
package: take the compiled code and package it in its distributable format, such as a JAR.
integration-test: process and deploy the package if necessary into an environment where integration tests can be run
verify: run any checks to verify the package is valid and meets quality criteria
install: install the package into the local repository, for use as a dependency in other projects locally
deploy: done in an integration or release environment, copies the final package to the remote repository for sharing with other developers and projects.
There are two other Maven lifecycles of note beyond the default list above. They are

clean: cleans up artifacts created by prior builds
site: generates site documentation for this project
Phases are actually mapped to underlying goals. The specific goals executed per phase is dependant upon the packaging type of the project. For example, package executes jar:jar if the project type is a JAR, and war:war if the project type is - you guessed it - a WAR.

An interesting thing to note is that phases and goals may be executed in sequence.

# developers ttypically use the node package manager (npm) to install software for coding
``` npm install
    npm start
    ```
# Sys Admin typically use other deployment tools [ local shares, servers, msi downloads, chocolately]
``` choco install
```


