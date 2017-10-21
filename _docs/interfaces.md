---
permalink: /interfaces/
---

# Interfaces

Interfaces 描述 value 的外形

```ts
class Clock implements IClockInterface {}
```

按惯例，interfaces 的名字以 'I' 开始。

## Object types

```ts
interface ISearchFunc {
  // 用 call signature 描述 function type
  (source: string, subString: string): boolean;
}

let mySearch: ISearchFunc = function (src, sub) {
  let result = src.search(sub);
  return result > -1;
}
```



## Function types

描述 function types

```ts
interface ISearchFunc {
  // 用 call signature 描述 function type
  (source: string, subString: string): boolean;
}

let mySearch: ISearchFunc = function (src, sub) {
  let result = src.search(sub);
  return result > -1;
}
```

函数参数的名字可以跟 call signature  不一样。

函数参数和返回值可以省略 types, 让 compiler 推断。

## Indexable Types



## Class Types

Interfaces 可以被 class 实现，一个 class 只能实现一个 interface。

```ts
class Clock implements IClockInterface {}
```

## extends

Interfaces 可以继承，并且一个 interface 可以继承多个 interfaces。

```ts
interface ISquare extends IShape, IPenStroke {}
```
