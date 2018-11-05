# IMPORTANT

This repository is not maintained anymore. It has been moved to https://github.com/paritytech/js-libs/tree/master/packages/abi.

# @parity/abi

A port of [https://github.com/paritytech/ethabi](https://github.com/paritytech/ethabi) to JavaScript

[![Build Status](https://travis-ci.org/paritytech/js-abi.svg?branch=master)](https://travis-ci.org/paritytech/js-abi)
[![Coverage Status](https://coveralls.io/repos/github/paritytech/js-abi/badge.svg?branch=master)](https://coveralls.io/github/paritytech/js-abi?branch=master)
[![Dependency Status](https://david-dm.org/paritytech/js-abi.svg)](https://david-dm.org/paritytech/js-abi)
[![devDependency Status](https://david-dm.org/paritytech/js-abi/dev-status.svg)](https://david-dm.org/paritytech/js-abi#info=devDependencies)

## contributing

Clone the repo and install dependencies via `npm install`. Tests can be executed via `npm run test`

## installation

Install the package with `npm install --save @parity/abi` from [@parity/abi](https://www.npmjs.com/package/@parity/abi)


## implementation
### approach

- this version tries to stay as close to the original Rust version in intent, function names & purpose
- it is a basic port of the Rust version, relying on effectively the same test-suite (expanded where deemed appropriate)
- it is meant as a library to be used in other projects, i.e. [@parity/api](https://www.npmjs.com/package/@parity/api)

### differences to original Rust version

- internally the library operates on string binary representations as opposed to Vector bytes, lengths are therefore 64 bytes as opposed to 32 bytes
- function names are adapted from the Rust standard snake_case to the JavaScript standard camelCase
- due to the initial library focus, the cli component (as implemented by the original) is not supported nor implemented
