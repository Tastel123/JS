## async
async 函数就是 Generator 函数的语法糖。

## generator
```js
function* test() {
            let a = yield 1
            console.log(a)
            let b = yield 2
            console.log(b)
            let c = yield 3
            console.log(c)
        }
        var g = test()
```
通过 g.next() 一步一步调用
每一步调用 执行到 yield 关键字
通过传参 作为上一个 yield 语句的返回值

## Promise.resolve
返回Promise
1. 如果是一个 Promise 返回一个 Promise
2. 如果是一个值 该值