# To reproduce issue

```console
$ yarn install

$ yarn build

warn  - React 17.0.1 or newer will be required to leverage all of the upcoming features in Next.js 11. Read more: https://err.sh/next.js/react-version
info  - Creating an optimized production build
Failed to compile.

ModuleNotFoundError: Module not found: Error: Can't resolve 'process' in '/Users/jacobwgillespie/with-styled-components-app/.yarn/$$virtual/styled-components-virtual-f1e74dcdfb/0/cache/styled-components-npm-5.2.1-e180c24b63-c27911be08.zip/node_modules/styled-components/dist'
BREAKING CHANGE: webpack < 5 used to include polyfills for node.js core modules by default.
This is no longer the case. Verify if you need this module and configure a polyfill for it.

If you want to include a polyfill, you need to:
	- add a fallback 'resolve.fallback: { "process": require.resolve("process/browser") }'
	- install 'process'
If you don't want to include a polyfill, you can use an empty module like this:
	resolve.fallback: { "process": false }


> Build error occurred
Error: > Build failed because of webpack errors
    at /Users/jacobwgillespie/with-styled-components-app/.yarn/$$virtual/next-virtual-f6d8a4bf57/0/cache/next-npm-10.0.7-387b04ca71-bea4fd15b2.zip/node_modules/next/dist/build/index.js:15:918
    at async /Users/jacobwgillespie/with-styled-components-app/.yarn/$$virtual/next-virtual-f6d8a4bf57/0/cache/next-npm-10.0.7-387b04ca71-bea4fd15b2.zip/node_modules/next/dist/build/tracer.js:3:470
```
