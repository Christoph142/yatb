Yet some other Terminate Buttons for Eclipse
====

This plugin adds four buttons to the Eclipse console. Two for each kind of shutdown mentioned below.
One of each set is for the active console, the other one to rule them all.

## Why

### Soft shutdown
Sometimes there are clean up tasks when shutting down certain processes.
Eclipse however doesn't signal a normal shutdown and hence doesn't trigger these tasks.
That's why this new button here. It will signal the process a normal shutdown request with `kill -SIGTERM` internally for Linux-like and OSX platforms.

### Hard shutdown
Sometimes processes are busy and don't react to the default shutdown action of Eclipse.
The buttons make it possible to send a `kill -SIGKILL` signal to them.

## Installation

1. Download the dist folder in this repository
2. Install [Maven](https://maven.apache.org/) if you don't have it
3. Open a terminal in the project root and run `mvn package` 
2. in Eclipse open Help -> Install new Software... -> Add... -> Local...
3. Select the site/target/site folder
4. Select the plugin and proceed like normal

Based on the original YaTB plugin by Nick Tan.
