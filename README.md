# SWC Minify Bug

## In dev, see the array content rendered
1. `npm run dev`
2. Open `http://localhost:3000`
3. See: `neverUndefined value: "[1,2]"`

## In prod, see the array content being empty
1. `npm run build && npm start`
2. Open `http://localhost:3000`
3. See: `neverUndefined value: ""`

## In prod, with `swcMinify:false`, see the array content rendered

1. Change `swcMinify` to false in next.config.js
2. `npm run build && npm start`
3. Open `http://localhost:3000`
4. See: `neverUndefined value: "[1,2]"`
