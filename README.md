# Demo webpack + deck.gl-leaflet

Run `npm run serve` to start webpack-dev-server

Open developer tools in browser.

See the error:
```
caught TypeError: Class extends value undefined is not a constructor or null
    at eval (deck.gl-leaflet.umd.min.js:2:1115)
    at eval (deck.gl-leaflet.umd.min.js:2:210)
    at eval (deck.gl-leaflet.umd.min.js:2:295)
    at ./node_modules/deck.gl-leaflet/dist/deck.gl-leaflet.umd.min.js (main.js:179:1)
    at __webpack_require__ (main.js:206:32)
    at fn (main.js:401:21)
    at eval (index.js:2:73)
    at ./src/index.js (main.js:168:1)
    at __webpack_require__ (main.js:206:32)
    at main.js:1272:37
```

Remove `"browser": "dist/deck.gl-leaflet.umd.min.js",` from `node_modules/deck.gl-leaflet/package.json`.
Restart `npm run serve`.
