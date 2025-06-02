## export-svg-typescript

Convert a folder of SVG icons into a color-customizable, tree-shakable TypeScript export `index.ts` that works with any component framework without SVG or Vite compiler issues.

1. Barrel Roll: Exports all icons as named functions for tree shaking to only the ones actually used.
2. Typescript Tooltip Previews: Each export includes a tooltip preview of icon.
3. Customizable: Change icon colors, size, and dimensions at runtime. Can return SVG or IMG tag with SVG as source.
4. CLI Tool: Use directly from the command line or in npm scripts.

### Install
Global install:
```
npm install -g export-svg-typescript
Or add to package.json:
```
 "icons": "npx export-svg-typescript -i ./src/icons",
```
Or use npx without installing globally with index output file set
```
 "icons": "npx export-svg-typescript ./src/icons",
```

### Example

Clone this repo and run `npm run demo` to see icons in demo folder.

```javascript
import { loadingDoubleRing } from './demo';

loadingDoubleRing({size: 200, colors: ["#5345bb"] })
```
![screenshot](https://i.imgur.com/aXczCC2.png)
