# @esm2cjs/slash

This is a fork of https://github.com/sindresorhus/slash, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i slash@npm:@esm2cjs/slash
```

```jsonc
// package.json
"dependencies": {
    "slash": "npm:@esm2cjs/slash"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/slash
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/slash": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import slash from "@esm2cjs/slash";

// Using CommonJS require()
const slash = require("@esm2cjs/slash").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/slash).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/slash).
