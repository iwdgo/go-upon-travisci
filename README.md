[![Build Status](https://api.cirrus-ci.com/github/iwdgo/go-upon-ci.svg)](https://cirrus-ci.com/github/iWdGo/go-upon-ci)

# Toolchain of go lang on tip

Toolchain runs the last commit on the `master` branch of go repository.
Yaml file has the standard name of the CI.
 - Build is executed using `make.bash`
 - Test is executed using `go tool dist test` 
 
## Cirrus CI

Toolchain is using the default container of golang:latest.
If any test fails, the job is marked as failed.
The artefact is available for download inside the Cirrus CI job. 
