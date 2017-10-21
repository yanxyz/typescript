---
permalink: /types/
---

# Types

```ts
let isDone: boolean = false
let count: number = 0
let color: string = 'blue'
```

注意，如果 type 为 Boolean, Number, String，表示的是 box object。

any 表示未知 type, compiler 不检查它。

```ts
let notSure: any = 4
notSure.toFixed(); // okay
```



## Functions


void 表示函数返回值为 null 或 undefined。

never 表示函数不能正常退出

```


```
