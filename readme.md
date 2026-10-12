# `robins-tsconfig`

[![latest version](https://npmx.dev/api/registry/badge/version/robins-tsconfig)](https://npmx.dev/robins-tsconfig)
[![npm downloads](https://npmx.dev/api/registry/badge/downloads/robins-tsconfig)](https://npmx.dev/robins-tsconfig)
[![license](https://npmx.dev/api/registry/badge/license/robins-tsconfig)](https://npmx.dev/robins-tsconfig)

> this is how i like my typescript projects. you might like it too. 🫱🏼‍🫲🏽

a quite strict [`tsconfig.json`](https://www.typescriptlang.org/tsconfig) to [extend](https://www.typescriptlang.org/tsconfig/#extends) from.

## installation & usage

```sh
npm i -D robins-tsconfig
```

```json
{
  "extends": "robins-tsconfig",
  "include": ["your", "includes", "here"],
  "exclude": ["your", "excludes", "here"]
}
```

## good to know

- the config makes use of defaults and implicit values as of typescript 6
- i borrowed heavily from [`@tsconfig/strictest`](https://npmx.dev/package/@tsconfig/strictest) and the [tsconfig cheat sheet](https://www.totaltypescript.com/tsconfig-cheat-sheet)
- you'll have to set [`include`](https://www.typescriptlang.org/tsconfig/#include) and [`exclude`](https://www.typescriptlang.org/tsconfig/#exclude) yourself for better performance
- it assumes you're building for the browser; change [`lib`](https://www.typescriptlang.org/tsconfig/#lib) if you're not
- if you want to compile via [`tsc`](https://www.typescriptlang.org/docs/handbook/compiler-options.html), override [`noEmit`](https://www.typescriptlang.org/tsconfig/#noEmit), [`outDir`](https://www.typescriptlang.org/tsconfig/#outDir) and [`rootDir`](https://www.typescriptlang.org/tsconfig/#rootDir)

## license

[mit](https://opensource.org/license/MIT)
