//[arrow-fx-stm](../../../index.md)/[arrow.fx.stm.internal](../index.md)/[Hamt](index.md)

# Hamt

[common]\
data class [Hamt](index.md)&lt;[A](index.md)&gt;(branches: [TVar](../../arrow.fx.stm/-t-var/index.md)&lt;[Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)&lt;[Branch](../-branch/index.md)&lt;[A](index.md)&gt;?&gt;&gt;)

Low level stm datastructure which can be used to efficiently implement other datastructures like Map/Set on top.

Based on http://lampwww.epfl.ch/papers/idealhashtrees.pdf and https://hackage.haskell.org/package/stm-hamt.

## Constructors

| | |
|---|---|
| [Hamt](-hamt.md) | [common]<br>fun &lt;[A](index.md)&gt; [Hamt](-hamt.md)(branches: [TVar](../../arrow.fx.stm/-t-var/index.md)&lt;[Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)&lt;[Branch](../-branch/index.md)&lt;[A](index.md)&gt;?&gt;&gt;) |

## Types

| Name | Summary |
|---|---|
| [Companion](-companion/index.md) | [common]<br>object [Companion](-companion/index.md) |

## Properties

| Name | Summary |
|---|---|
| [branches](branches.md) | [common]<br>val [branches](branches.md): [TVar](../../arrow.fx.stm/-t-var/index.md)&lt;[Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)&lt;[Branch](../-branch/index.md)&lt;[A](index.md)&gt;?&gt;&gt; |
