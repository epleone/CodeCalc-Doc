
# 字符串


- `str(x)` : 将输入的值转换为字符串
- `num(x)` : 将输入的值转换为数字
- `upper(x)` : 将字符串转换为大写, 支持属性调用, 也就是 "x.upper" 等价于 upper(x)
- `lower(x)` : 将字符串转换为小写, 支持属性调用 ".lower"
- `length(x)` : 获取字符串的长度, 支持属性调用 ".length"
- `base64(x)` : 对字符串进行Base64编码, 支持属性调用 ".base64"
- `unbase64(x)` : 对字符串进行Base64解码, 支持属性调用 ".unbase64"


``` js
// 三种字符串定义方式
"hello", 'hello', `hello`

// 使用str函数得到字符串，括号内的值都会被转成字符串
str("hello") // 得到字符串`"hello"`, 包括引号。

upper("hello")          // 输出: "HELLO"
lower("HELLO")          // 输出: "hello"
length("hello")         // 输出: 5
base64("hello")         // 输出: "aGVsbG8="
unbase64("aGVsbG8=")    // 输出: "hello"

// 这些函数都支持属性调用
"hello".upper           // 输出: "HELLO"
"HELLO".lower           // 输出: "hello"
"hello".length          // 输出: 5
"hello".base64          // 输出: "aGVsbG8="
"aGVsbG8=".unbase64     // 输出: "hello"

// 可以配合变量使用
a = "hello"
a.upper()   // 输出: "HELLO"

b = str("world")
b.upper()   // 输出: "WORLD"

a + b       // 输出: "helloworld"
```


![[image20250118233135.png]] { width="50%"}