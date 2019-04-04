# ESM import @babel/core bug repro

### Summary

Using `esm` to import `@babel/core` does not work when executing node scripts using the node CLI.

You can test this by running `yarn test` in this repo.

However, the import works from the node repl

```js
> require("esm")(module)
> import { transformFileAsync } from '@babel/core';
```