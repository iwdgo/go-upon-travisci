[![Build Status](https://travis-ci.com/iwdgo/go-upon-ci.svg?branch=master)](https://travis-ci.com/iWdGo/go-upon-ci)

# Toolchain of go lang on tip

Toolchain runs the last commit on the `master` branch.
Yaml file has the standard name of the CI.
 - Build is executed using `make.bash`
 - Test is executed using `go tool dist test` 

## Travis CI 

Toolchain runs on default architecture `amd64` on Linux, Windows and OSX.
Status is on build. Badge does not report a failing test.
For an unknown reason, it is necessary to tailor the last line of make.bash.
