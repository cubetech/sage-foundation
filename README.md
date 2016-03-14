# How to replace Bootstrap with [Foundation for Roots/Sage](https://github.com/roots/sage)

## 1. Clone, clean and install

* Clone repo: `git clone https://github.com/roots/sage.git`
* Remove Bootstrap: `bower uninstall bootstrap-sass -S`
* Install Foundation: `bower install foundation -S`
* Install NPM packages: `npm install`

## 2. Add Foundation overrides to `bower.json` like this:

```
  "overrides": {
    "foundation": {
      "main": [

        "./scss/normalize.scss",
        "./scss/foundation.scss",


        "../fastclick/lib/fastclick.js",

    
        "./js/foundation/foundation.js",
        "./js/foundation/foundation.abide.js",
        "./js/foundation/foundation.accordion.js",
        "./js/foundation/foundation.alert.js",
        "./js/foundation/foundation.clearing.js",
        "./js/foundation/foundation.dropdown.js",
        "./js/foundation/foundation.equalizer.js",
        "./js/foundation/foundation.interchange.js",
        "./js/foundation/foundation.joyride.js",
        "./js/foundation/foundation.magellan.js",
        "./js/foundation/foundation.offcanvas.js",
        "./js/foundation/foundation.orbit.js",
        "./js/foundation/foundation.reveal.js",
        "./js/foundation/foundation.slider.js",
        "./js/foundation/foundation.tab.js",
        "./js/foundation/foundation.tooltip.js",
        "./js/foundation/foundation.topbar.js"

      ]
    }
    
  }
```

## 3. Comment out Bootstrap sass stuff in `assets/styles/main.scss`

## 4. Replace dev url in `assets/manifest.json` and lastly run `gulp watch`

