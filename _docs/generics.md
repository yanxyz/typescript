---
permalink: /generics/
---

# Generics

## Generic functions

```ts
function identity(arg: any): any {
  return arg;
}
// output 的 type 为 any，这没意义
let output = identity(1);
```

使用泛型

```ts
function identity<T>(arg: T): T {
  return arg;
}
// output 的 type 为 number
let output = identity(1);
```

在定义泛型时，T 为 type variable，用于 types 而不用于 values。

在使用泛型时，有两种方式

```ts
let x = identity<number>(1);
let y = identity(1); // type argument inference
```

通常省略 type, 让 compiler 推断。如果 compiler 失败，再明确指定 type。

## Generic Types


-
- [Generic Classes](https://www.typescriptlang.org/docs/handbook/generics.html#generic-classes)

