# Installation and quickstart

# Installation on OSX

## Build environment

- `brew install leiningen`

## Editor

- If you already have an installation of IntelliJ then you can just install the plugin
    - Go to plugins, search for `Cursive`, and click on install
- If you don't have IntelliJ then you can download the the IDE from the website: [Cursive](https://cursive-ide.com/userguide/)

You'll also need a non-commercial license, which you'll need to obtain from the website [here](https://cursive-ide.com/buy.html). A non-commercial license is fine for hobby projects
and lasts twelve months, after which you can just download another license.

One of the things that makes editing Clojure code more pleasurable is Paredit mode, where the editor keeps parenthesis balanced for you. There is
a good explanation of the various operations on the Cursive site here: [Paredit mode](https://cursive-ide.com/userguide/paredit.html).

# Running the REPL

## From the command line

- Start the REPL: `lein repl`
- Exit the REPL: `CTRL-d`

## Inside Cursive

- TBD 

# Getting starting

## Creating a basic project

- Leiningen can create starter projects from templates, such as the `app` template which is a simple application:
    - `lein new app my-project-name`
