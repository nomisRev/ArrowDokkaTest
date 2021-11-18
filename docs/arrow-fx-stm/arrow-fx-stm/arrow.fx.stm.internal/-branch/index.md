//[arrow-fx-stm](../../../index.md)/[arrow.fx.stm.internal](../index.md)/[Branch](index.md)

# Branch

[common]\
sealed class [Branch](index.md)&lt;out [A](index.md)&gt;

## Types

| Name | Summary |
|---|---|
| [Branches](-branches/index.md) | [common]<br>data class [Branches](-branches/index.md)&lt;[A](-branches/index.md)&gt;(sub: [Hamt](../-hamt/index.md)&lt;[A](-branches/index.md)&gt;) : [Branch](index.md)&lt;[A](-branches/index.md)&gt; |
| [Leaf](-leaf/index.md) | [common]<br>data class [Leaf](-leaf/index.md)&lt;[A](-leaf/index.md)&gt;(hash: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html), value: [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)&lt;[Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)?&gt;) : [Branch](index.md)&lt;[A](-leaf/index.md)&gt; |

## Inheritors

| Name |
|---|
| [Branch](-branches/index.md) |
| [Branch](-leaf/index.md) |
