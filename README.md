[![Build Status](https://travis-ci.com/iWdGo/go-upon-ci.svg?branch=master)](https://travis-ci.com/iWdGo/go-upon-ci)
[![Build Status](https://api.cirrus-ci.com/github/iWdGo/go-upon-ci.svg)](https://cirrus-ci.com/github/iWdGo/go-upon-ci)
![Build status](https://github.com/iWdGo/go-upon-ci/workflows/Go/badge.svg)

# Toolchain of go lang on tip

Toolchain runs the last commit on the `master` branch.
Yaml file has the standard name of the CI.
 - Build is executed using `make.bash`
 - Test is executed using `go tool dist test` 
 
## Cirrus CI

Toolchain is using the default container of golang:latest.
If any test fails, the job is marked as failed.
The artefact is available for download inside the Cirrus CI job. 

## Travis CI 

Toolchain runs on Linux and Windows on the default architecture `amd64`.
Status is on build. Any failing test is not reported by the badge.
For an unknown reason, it is necessary to override make.bash.

## Github Actions

Toolchain runs on Ubuntu on `amd64` which is the default image.

## Issue branch

To build a patched version using tip:
- Add a patch file to the `issue<#issue number>` branch using `git format-patch <your commit>` 
- Push to your published repository.