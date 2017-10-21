---
permalink: /arrays/
---

# Arrays

Array type

```ts
let a: number[]
```

泛型，`Array<T>` type，同上

```ts
let a: Array<number>
```

泛型，`ReadonlyArray<T>` type，不可以修改数组及其元素

```ts
let a: number[] = [1, 2, 3, 4];
let ro: ReadonlyArray<number> = a; // Array<T> => ReadonlyArray<T>
ro[0] = 12; // error!
ro.push(5); // error!
ro.length = 100; // error!
a = ro; // error!
a = ro as number[]; // ReadonlyArray<T> => Array<T>
```
