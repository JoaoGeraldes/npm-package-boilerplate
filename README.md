# Development

### 📦 BUILD (builds to /dist directory)

#### Without compress/minification
1. npm run build

#### With compress/minification
2. npm-run-all build minify

### 🔂 Increment version before publishing package

npm version patch

#### Test locally, before publish

- (within the project's directory)
  - `npm run build` or `npm-run-all build minify`
  - `npm link`
- (outside the project's directory - somewhere else to test our latest package changes)
  - `npm link cherrylog` (mimics the _npm install cherrylog_)
  - `import cherrylog from "cherrylog"`