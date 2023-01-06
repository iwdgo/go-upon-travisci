[![Build Status](https://app.travis-ci.com/iwdgo/go-upon-ci.svg?branch=travisci)](https://app.travis-ci.com/iwdgo/go-upon-ci)

# Toolchain of go lang on tip on Travis CI

Toolchain runs the last commit on the `master` branch.
Yaml file has the standard name of the CI.
 - Build is executed using `make.bash`
 - Test is executed using `go tool dist test` 

Toolchain runs on default architecture `amd64` on Linux, Windows and OSX.  

Status is on build. 
