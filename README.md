# shopSFI

### Setup

##### Prerequisites

Install [polymer-cli](https://github.com/Polymer/polymer-cli):

    npm install -g polymer-cli

Need at least node v0.3.0

##### Setup

    git clone https://github.com/oneezy/shopSFI.git
    cd shopSFI
    bower install

### Start the development server

    polymer serve

### Run web-component-tester tests

    polymer test

### Build

    polymer build

### Test the build

This command serves the minified version of the app in an unbundled state, as it would be served by a push-compatible server:

    polymer serve build/unbundled

This command serves the minified version of the app generated using fragment bundling:

    polymer serve build/bundled
