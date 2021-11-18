//[arrow-fx-coroutines](../../../index.md)/[arrow.fx.coroutines](../index.md)/[Use](index.md)

# Use

[common]\
~~inline~~ ~~class~~ [~~Use~~](index.md)~~&lt;~~[A](index.md)~~&gt;~~~~(~~~~acquire~~~~:~~ suspend () -&gt; [A](index.md)~~)~~

Marker for suspend () -&gt; A to be marked as the [Use](index.md) action of a [Resource](../-resource/index.md). Offers a convenient DSL to use [Resource](../-resource/index.md) for simple resources.

import arrow.fx.coroutines.*\
\
class File(url: String) {\
  suspend fun open(): File = this\
  suspend fun close(): Unit {}\
  override fun toString(): String = "This file contains some interesting content!"\
}\
\
suspend fun openFile(uri: String): File = File(uri).open()\
suspend fun closeFile(file: File): Unit = file.close()\
suspend fun fileToString(file: File): String = file.toString()\
\
suspend fun main(): Unit {\
  val res = resource {\
    openFile("data.json")\
  } release { file -&gt;\
    closeFile(file)\
  } use { file -&gt;\
    fileToString(file)\
  }\
\
  println(res)\
}<!--- KNIT example-resource-09.kt -->

## Constructors

| | |
|---|---|
| [Use](-use.md) | [common]<br>fun &lt;[A](index.md)&gt; [Use](-use.md)(acquire: suspend () -&gt; [A](index.md)) |

## Extensions

| Name | Summary |
|---|---|
| [release](../release.md) | [common]<br>~~infix~~ ~~fun~~ ~~&lt;~~[A](../release.md)~~&gt;~~ [Use](index.md)&lt;[A](../release.md)&gt;~~.~~[~~release~~](../release.md)~~(~~~~release~~~~:~~ suspend ([A](../release.md)) -&gt; [Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)~~)~~~~:~~ [Resource](../-resource/index.md)&lt;[A](../release.md)&gt; |
| [releaseCase](../release-case.md) | [common]<br>~~infix~~ ~~fun~~ ~~&lt;~~[A](../release-case.md)~~&gt;~~ [Use](index.md)&lt;[A](../release-case.md)&gt;~~.~~[~~releaseCase~~](../release-case.md)~~(~~~~release~~~~:~~ suspend ([A](../release-case.md), [ExitCase](../-exit-case/index.md)) -&gt; [Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)~~)~~~~:~~ [Resource](../-resource/index.md)&lt;[A](../release-case.md)&gt; |
