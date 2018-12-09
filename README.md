# colors

Is a basic console color library intended for [Deno](https://deno.land/). It is
inspired by packages like [chalk](https://www.npmjs.com/package/chalk) and
[colors](https://www.npmjs.com/package/colors) on npm.

## Usage

The main modules exports a single function name `color` which is a function
that provides chaining to stack colors. Basic usage looks like this:

```ts
import { color } from "https://deno.land/x/colors/main.ts";

console.log(color.bgBlue.red.bold("Hello world!"));
```

## TODO

- Currently, it just assumes it is running in an environment that supports ANSI
  escape code terminal coloring. It should actually detect, specifically
  windows and adjust properly.

- Test coverage is very basic at the moment.

---

Licensed under the [MIT License](./LICENSE).

Copyright 2018 — Kitson P. Kelly — All Rights Reserved.
