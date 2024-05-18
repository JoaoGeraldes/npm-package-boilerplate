# 🔎 Description
**NPM Package Boilerplate: The Quick Start Kit for Lazy Geniuses!**

Welcome to the ultimate boilerplate for those who want to get straight to the coding action without the hassle! This setup is so smooth, you might start believing in magic. Pre-configured with **TypeScript** and automatic **minification**, it’s the perfect toolkit for anyone who wants to get the boring stuff out of the way with minimal effort.

**Start your own npm package library today!** 🚀


# 1. 💻 Develop 

1. Create a new project folder and copy the contents of this repository into it.
2. If you want to modify the default (`index.js`) name for your entry file (compiled/built), make sure to change it on the `package.json` file.
3. Change the `name` property in the `package.json` to your desired package name.
4. Start developing your package at `src/index.ts`.

# 2. 📦 Build (`/dist`)

1. **Without compression/minification**

   `npm run build`

2. **With compression/minification**

   `npm-run-all build minify`

   By default, your compiled version goes to `/dist` directory.

# 3. 🚀 Publish

### 1. Test locally (before publish)

_within the project's directory_

1. `npm run build` or `npm-run-all build minify`
1. `npm link`

   _outside the project's directory - somewhere else to test our latest package changes_

1. `npm link my-package` (mimics the _npm install my-package_)

1. ```js
   import myPackage from "my-package";
   ```

### 2. Deploy to npm (https://www.npmjs.com/)

1. Increment version before publishing

   `npm version patch`

1. Build (with or without compression)

   `npm-run-all build minify` or `npm run build`

1. Deploy to npm

   `npm publish`
