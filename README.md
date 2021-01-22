TypeScript Snowpack React PostCss Issue Demo
=================================

If the postcss file has custom extension, e.g. `.pcss` other than '.css', even if we have configured 
`@snowpack/plugin-postcss` with `input: ['.pcss']`, it doesn't work.

```
npm install
npm run demo
```

On the opened page, the postcss defined in `index.pcss` are not applied.

If you change `index.pcss` to `index.css` and remove configuration of `input: ['.pcss']`, it will be OK. 
