[![Build Status](https://travis-ci.com/iWdGo/go-upon-ci.svg?branch=master)](https://travis-ci.com/iWdGo/go-upon-ci)
[![Build Status](https://api.cirrus-ci.com/github/iWdGo/go-upon-ci.svg)](https://cirrus-ci.com/github/iWdGo/go-upon-ci)

# Build go lang on tip

On the master branch, yaml for CI to build and test `go` lang on tip.
 - Build is done using `make.bash`
 - Test is executed using `go tool dist` 
 
## Cirrus CI

Build is using the default container of golang:latest.
The artefact is available for download inside the Cirrus CI job. 

## Travis CI 

Build on Linux and Windows.
Default architecture is `amd64`

## Issue branch

To build a patched version using tip:
- Add a patch file to a relevant branch using `git format-patch <your commit>` 
- Push to your published repository.