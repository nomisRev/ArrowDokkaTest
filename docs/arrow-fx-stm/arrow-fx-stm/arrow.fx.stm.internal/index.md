//[arrow-fx-stm](../../index.md)/[arrow.fx.stm.internal](index.md)

# Package arrow.fx.stm.internal

## Types

| Name | Summary |
|---|---|
| [BlockedIndefinitely](-blocked-indefinitely/index.md) | [common]<br>class [BlockedIndefinitely](-blocked-indefinitely/index.md) : [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)<br>In some special cases it is possible to detect if a STM transaction blocks indefinitely so we can abort here. |
| [Branch](-branch/index.md) | [common]<br>sealed class [Branch](-branch/index.md)&lt;out [A](-branch/index.md)&gt; |
| [Hamt](-hamt/index.md) | [common]<br>data class [Hamt](-hamt/index.md)&lt;[A](-hamt/index.md)&gt;(branches: [TVar](../arrow.fx.stm/-t-var/index.md)&lt;[Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)&lt;[Branch](-branch/index.md)&lt;[A](-hamt/index.md)&gt;?&gt;&gt;)<br>Low level stm datastructure which can be used to efficiently implement other datastructures like Map/Set on top. |
| [RetryException](-retry-exception/index.md) | [common, js, jvm, native]<br>[common, js, jvm, native]<br>object [RetryException](-retry-exception/index.md) : [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html) |

## Functions

| Name | Summary |
|---|---|
| [alterHamtWithHash](alter-hamt-with-hash.md) | [common]<br>inline fun &lt;[A](alter-hamt-with-hash.md)&gt; [STM](../arrow.fx.stm/-s-t-m/index.md).[alterHamtWithHash](alter-hamt-with-hash.md)(hamt: [Hamt](-hamt/index.md)&lt;[A](alter-hamt-with-hash.md)&gt;, hash: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html), test: ([A](alter-hamt-with-hash.md)) -&gt; [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html), fn: ([A](alter-hamt-with-hash.md)?) -&gt; [A](alter-hamt-with-hash.md)?): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [atDepth](at-depth.md) | [common]<br>fun [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html).[atDepth](at-depth.md)(d: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [clearHamt](clear-hamt.md) | [common]<br>fun &lt;[A](clear-hamt.md)&gt; [STM](../arrow.fx.stm/-s-t-m/index.md).[clearHamt](clear-hamt.md)(hamt: [Hamt](-hamt/index.md)&lt;[A](clear-hamt.md)&gt;) |
| [index](--index--.md) | [common]<br>fun [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html).[index](--index--.md)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [indexAtDepth](index-at-depth.md) | [common]<br>fun [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html).[indexAtDepth](index-at-depth.md)(d: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [lookupHamtWithHash](lookup-hamt-with-hash.md) | [common]<br>inline fun &lt;[A](lookup-hamt-with-hash.md)&gt; [STM](../arrow.fx.stm/-s-t-m/index.md).[lookupHamtWithHash](lookup-hamt-with-hash.md)(hmt: [Hamt](-hamt/index.md)&lt;[A](lookup-hamt-with-hash.md)&gt;, hash: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html), test: ([A](lookup-hamt-with-hash.md)) -&gt; [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)): [A](lookup-hamt-with-hash.md)? |
| [newHamt](new-hamt.md) | [common]<br>fun &lt;[A](new-hamt.md)&gt; [STM](../arrow.fx.stm/-s-t-m/index.md).[newHamt](new-hamt.md)(): [Hamt](-hamt/index.md)&lt;[A](new-hamt.md)&gt; |
| [nextDepth](next-depth.md) | [common]<br>fun [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html).[nextDepth](next-depth.md)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [pair](pair.md) | [common]<br>fun &lt;[A](pair.md)&gt; [STM](../arrow.fx.stm/-s-t-m/index.md).[pair](pair.md)(depth: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html), hash1: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html), branch1: [Branch](-branch/index.md)&lt;[A](pair.md)&gt;, hash2: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html), branch2: [Branch](-branch/index.md)&lt;[A](pair.md)&gt;): [Hamt](-hamt/index.md)&lt;[A](pair.md)&gt; |

## Properties

| Name | Summary |
|---|---|
| [ARR_SIZE](-a-r-r_-s-i-z-e.md) | [common]<br>const val [ARR_SIZE](-a-r-r_-s-i-z-e.md): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) = 32 |
| [DEPTH_STEP](-d-e-p-t-h_-s-t-e-p.md) | [common]<br>const val [DEPTH_STEP](-d-e-p-t-h_-s-t-e-p.md): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) = 5 |
| [MASK](-m-a-s-k.md) | [common]<br>const val [MASK](-m-a-s-k.md): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
