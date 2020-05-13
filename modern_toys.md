# 1.摩登玩具

---

`5` 是一个整数吗？

*是的。*

---

`-23` 是数字吗？

*是的，但我们不会用到负整数。*

---

`5.32` 是一个整数吗？

*不是，我们也不会用到这种类型的数字。*

---

数字 `5` 是什么类型？

*`int`*

---

快，想个其它整数！

*`19` 怎么样？*

---

`true` 是什么类型的值？

*`boolean`*

---

`false` 是什么类型的值？

*`boolean`*

---

除此之外，你还能想到其它 `boolean` 类型的值吗？

*不能，这就是所有 `boolean` 类型的值了*

---

`int` 是什么？

*一种类型*

---

`boolean` 是什么？

*另一种类型*

---

什么是类型？

*类型指的是值的集合*

---

什么是类型？？

*有时我们把它当作是集合*

---

我们可以创建一个新的类型吗？

*我们还不知道怎么做。*

---

画出下列类间的关系图。

```java
abstract class Seasoning {}

class Salt extends Seasoning {}

class Pepper extends Seasoning {}
```

---

嗯，我们认为 `Seasoning` 是一种类型，而 `Salt` 和 `Pepper` 是它的变体。

*好的。不过，这三个类不也都是新的类型吗？*

---

某种意义上来说，是这样的。现在，`new Salt()` 是否返回一个 `Seasoning` 类型的值？

是的。因为 `new Salt()` 返回一个 `Salt` 的实例， 而每个 `Salt` 都属于 `Seasoning` 类型。

---

那么 `new Pepper()` 呢？

*也一样。`new Pepper()` 返回一个 `Pepper` 的实例， 而每个 `Pepper` 都属于 `Seasoning` 类型。*

---

`abstract`, `class` 和 `extends` 都是什么呀？

*简单。`abstract class` 引入一种数据类型，`class` 引入变体（派生类？），`entends` 把两者结合起来。*

---

还有没有其它的 `Seasoning` ？

*没有。因为只有 `Salt` 和 `Pepper` 继承了 `Seasoning`*

---

对的，`Salt` 和 `Pepper` 是 `Seasoning` 仅有的变体。我们还有遇到过像 `Seasoning` 这样的类型吗？

*没有了。不过，`boolean` 也是仅有两个值的数据类型。*

---

让我们来定义更多的 `Seasoning` 吧！

```Java
class Thyme extends Seasoning {}
```

*还可以有更多*

```Java
class Sage extends Seasoning {}
```

---

现在有四个了。

*是的。*

---

什么是笛卡尔点？

*两个数字的组合。*

---

曼哈顿的一个点表示什么？

*两条街道点相交之处*

---

`CartesianPt` 和 `ManhattanPt` 与 `Salt` 和 `Pepper` 有什么不同？

```Java
abstract class Point {}

class CartesianPt extends Point {
    int x;
    int y;
    CartesianPt(int _x, int _y) {
        x = _x;
        y = _y;
    }
}


class ManhattanPt extends Point {
    int x;
    int y;
    ManhattanPt(int _x, int _y) {
        x = _x;
        y = _y;
    }
}
```
