# Property Grid System `<fx-properties>`
----------------------
FX Properties is a grid system created with custom `[attribute="property"]'s` (just like the 90's!). <br>
The idea is to separate your *every day* page layout from your "deep" CSS custom styling. <br>
It's recommended to use Polymer, the web component polyfill (but not required)

 **DEMO:** http://oneezy.github.io/fx-properties (resize your browser)

----------------------

## Usage
Include this folder in your directory and put this file in your head
 - `<link rel="import" href="fx-properties.html">`

## Understanding

#### There are 4 `"universal"` CSS files:

 - `<link rel="import" href="properties/fx-grid.html">`
 - `<link rel="import" href="properties/fx-positioning.html">`
 - `<link rel="import" href="properties/fx-settings.html">`
 - `<link rel="import" href="properties/fx-typography.html">`


#### There 3 folders including 4 `"media query"` CSS files for each device:
 - `mobile ......... @media (min-width: 0) and (max-width: 768px)`
 - `tablet ......... @media (min-width: 769px) and (max-width: 1024px)`
 - `desktop ........ @media (min-width: 1025px)`

#### For each `[attribute="property"]`, there's an exact mirrored `media query` property:

 **EXAMPLE:**

```
<div grid="vertical" layout="center" flex="auto"
     bg="white"
     mobile-bg="blue"
     tablet-bg="yellow"
     desktop-bg="green">
</div>
```

<br>
<br>
<br>

That's it!

<br>
<br>

----------------------
## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
