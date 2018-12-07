# About this project #

We're going to build a little web service that verifies ISBN numbers.

# Getting started #

## Creating the project ##

- Create the project
    - `lein new duct isbn-verifier +api +example`
- Go into the directory
    - `cd isbn-verifier`
- Set up duct
    - `lein duct setup`
- Configure IntelliJ
    - `TODO`

## Running the project ##

- Run a REPL
    - `lein repl`
- Load the development environment

  ```clojure
  user=> (dev)
  :loaded
  ```

- Run `go` to prep and initiate the system.

  ```clojure
  dev=> (go)
  :duct.server.http.jetty/starting-server {:port 3000}
  :initiated
  ```

- Issue a `GET` request to retrieve some data:

  ```
  curl -X GET 'http://localhost:3000/example'
  {"example":"data"}
  ```

# Making changes #

The request routing is in `src/isbn_verifier/handler/example.clj` (the underscore is instead of a hyphen is not a
mistake -- the JVM doesn't handle hyphens in package names). You can change existing routes or add new routes there.

## Reloading after changes ##

- Restart the system when you change files using `reset`:

  ```clojure
  dev=> (reset)
  :reloading (...)
  :resumed
  ```

## Testing ##

- Use `test` to run the tests:

  ```clojure
  dev=> (test)
  ...
  ```

