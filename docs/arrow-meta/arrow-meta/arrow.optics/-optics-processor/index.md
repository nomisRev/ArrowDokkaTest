//[arrow-meta](../../../index.md)/[arrow.optics](../index.md)/[OpticsProcessor](index.md)

# OpticsProcessor

[jvm]\
@AutoService(value = [[Processor::class](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/Processor.html)])

class [OpticsProcessor](index.md) : [AbstractProcessor](../../arrow.common.utils/-abstract-processor/index.md)

## Functions

| Name | Summary |
|---|---|
| [asClassOrPackageDataWrapper](../../arrow.common.utils/-processor-utils/as-class-or-package-data-wrapper.md) | [jvm]<br>open fun KotlinMetadata.[asClassOrPackageDataWrapper](../../arrow.common.utils/-processor-utils/as-class-or-package-data-wrapper.md)(classElement: [TypeElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/TypeElement.html)): [ClassOrPackageDataWrapper](../../arrow.common.utils/-class-or-package-data-wrapper/index.md)? |
| [asModifier](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/as-modifier.md) | [jvm]<br>open fun ProtoBuf.Modality.[asModifier](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/as-modifier.md)(): [Modifier](../../arrow.meta.ast/-modifier/index.md)<br>open fun ProtoBuf.Visibility.[asModifier](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/as-modifier.md)(): [Modifier](../../arrow.meta.ast/-modifier/index.md)? |
| [asTypeName](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/as-type-name.md) | [jvm]<br>open fun ProtoBuf.Type.[asTypeName](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/as-type-name.md)(meta: [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md)): [TypeName](../../arrow.meta.ast/-type-name/index.md) |
| [declaredTypeClassInterfaces](../../arrow.common.utils/-processor-utils/declared-type-class-interfaces.md) | [jvm]<br>open fun [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md).[declaredTypeClassInterfaces](../../arrow.common.utils/-processor-utils/declared-type-class-interfaces.md)(typeTable: TypeTable): [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)&lt;[ClassOrPackageDataWrapper](../../arrow.common.utils/-class-or-package-data-wrapper/index.md)&gt; |
| [extractFullName](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/extract-full-name.md) | [jvm]<br>open fun ProtoBuf.Type.[extractFullName](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/extract-full-name.md)(classData: [ClassOrPackageDataWrapper](../../arrow.common.utils/-class-or-package-data-wrapper/index.md), outputTypeAlias: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) = true): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [getClassData](../../arrow.common.utils/-processor-utils/get-class-data.md) | [jvm]<br>open fun [Element](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/Element.html).[getClassData](../../arrow.common.utils/-processor-utils/get-class-data.md)(): [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md) |
| [getClassOrPackageDataWrapper](../../arrow.common.utils/-processor-utils/get-class-or-package-data-wrapper.md) | [jvm]<br>open fun [getClassOrPackageDataWrapper](../../arrow.common.utils/-processor-utils/get-class-or-package-data-wrapper.md)(classElement: [TypeElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/TypeElement.html)): [ClassOrPackageDataWrapper](../../arrow.common.utils/-class-or-package-data-wrapper/index.md) |
| [getCompletions](index.md#1387168281%2FFunctions%2F-35121544) | [jvm]<br>open override fun [getCompletions](index.md#1387168281%2FFunctions%2F-35121544)(element: [Element](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/Element.html)?, annotation: [AnnotationMirror](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/AnnotationMirror.html)?, member: [ExecutableElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ExecutableElement.html)?, userText: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)?): [Iterable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)&lt;[Completion](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/Completion.html)&gt; |
| [getConstructorParamNames](../../arrow.common.utils/-processor-utils/get-constructor-param-names.md) | [jvm]<br>open fun [Element](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/Element.html).[getConstructorParamNames](../../arrow.common.utils/-processor-utils/get-constructor-param-names.md)(): [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt; |
| [getConstructorTypesNames](../../arrow.common.utils/-processor-utils/get-constructor-types-names.md) | [jvm]<br>open fun [Element](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/Element.html).[getConstructorTypesNames](../../arrow.common.utils/-processor-utils/get-constructor-types-names.md)(): [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt; |
| [getFunction](../../arrow.common.utils/-processor-utils/get-function.md) | [jvm]<br>open fun [ClassOrPackageDataWrapper](../../arrow.common.utils/-class-or-package-data-wrapper/index.md).[getFunction](../../arrow.common.utils/-processor-utils/get-function.md)(methodElement: [ExecutableElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ExecutableElement.html)): ProtoBuf.Function? |
| [getFunctionOrNull](index.md#-1924364317%2FFunctions%2F-35121544) | [jvm]<br>open fun ClassData.[getFunctionOrNull](index.md#-1924364317%2FFunctions%2F-35121544)(methodElement: [ExecutableElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ExecutableElement.html)): ProtoBuf.Function?<br>open fun PackageData.[getFunctionOrNull](index.md#-644467023%2FFunctions%2F-35121544)(methodElement: [ExecutableElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ExecutableElement.html)): ProtoBuf.Function?<br>open fun [getFunctionOrNull](index.md#-2082541386%2FFunctions%2F-35121544)(methodElement: [ExecutableElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ExecutableElement.html), nameResolver: NameResolver, functionList: [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)&lt;ProtoBuf.Function&gt;): ProtoBuf.Function? |
| [getSupportedAnnotationTypes](get-supported-annotation-types.md) | [jvm]<br>open override fun [getSupportedAnnotationTypes](get-supported-annotation-types.md)(): [Set](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt; |
| [getSupportedOptions](index.md#1992178418%2FFunctions%2F-35121544) | [jvm]<br>open override fun [getSupportedOptions](index.md#1992178418%2FFunctions%2F-35121544)(): [Set](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt; |
| [getSupportedSourceVersion](get-supported-source-version.md) | [jvm]<br>open override fun [getSupportedSourceVersion](get-supported-source-version.md)(): [SourceVersion](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/SourceVersion.html) |
| [init](index.md#-1807153948%2FFunctions%2F-35121544) | [jvm]<br>open override fun [init](index.md#-1807153948%2FFunctions%2F-35121544)(processingEnv: [ProcessingEnvironment](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/ProcessingEnvironment.html)) |
| [isInitialized](index.md#-698599737%2FFunctions%2F-35121544) | [jvm]<br>open fun [isInitialized](index.md#-698599737%2FFunctions%2F-35121544)(): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [kDoc](../../arrow.common.utils/-abstract-processor/k-doc.md) | [jvm]<br>fun [Element](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/Element.html).[kDoc](../../arrow.common.utils/-abstract-processor/k-doc.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)? |
| [modifiersFromFlags](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/modifiers-from-flags.md) | [jvm]<br>open fun [modifiersFromFlags](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/modifiers-from-flags.md)(flags: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)): [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)&lt;[Modifier](../../arrow.meta.ast/-modifier/index.md)&gt; |
| [nameOf](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/name-of.md) | [jvm]<br>open fun [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md).[nameOf](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/name-of.md)(id: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [overrides](../../arrow.common.utils/-processor-utils/overrides.md) | [jvm]<br>open fun ProtoBuf.Function.[overrides](../../arrow.common.utils/-processor-utils/overrides.md)(o: ProtoBuf.Function): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [process](../../arrow.common.utils/-abstract-processor/process.md) | [jvm]<br>override fun [process](../../arrow.common.utils/-abstract-processor/process.md)(annotations: [Set](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)&lt;[TypeElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/TypeElement.html)&gt;, roundEnv: [RoundEnvironment](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/RoundEnvironment.html)): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [supertypes](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/supertypes.md) | [jvm]<br>open fun [supertypes](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/supertypes.md)(current: [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md), typeTable: TypeTable, processorUtils: [ProcessorUtils](../../arrow.common.utils/-processor-utils/index.md), acc: [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)&lt;[ClassOrPackageDataWrapper](../../arrow.common.utils/-class-or-package-data-wrapper/index.md)&gt;): [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)&lt;[ClassOrPackageDataWrapper](../../arrow.common.utils/-class-or-package-data-wrapper/index.md)&gt; |
| [toMeta](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/to-meta.md) | [jvm]<br>open fun ProtoBuf.Modality.[toMeta](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/to-meta.md)(): [Modifier](../../arrow.meta.ast/-modifier/index.md)<br>open fun ProtoBuf.TypeParameter.Variance.[toMeta](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/to-meta.md)(): [Modifier](../../arrow.meta.ast/-modifier/index.md)<br>open fun ProtoBuf.TypeParameter.[toMeta](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/to-meta.md)(owner: [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md)): [TypeName.TypeVariable](../../arrow.meta.ast/-type-name/-type-variable/index.md)<br>open fun ProtoBuf.ValueParameter.[toMeta](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/to-meta.md)(owner: [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md)): [Parameter](../../arrow.meta.ast/-parameter/index.md)<br>open fun ProtoBuf.Function.[toMeta](../../arrow.meta.encoder.jvm/-kotlin-metatadata-encoder/to-meta.md)(owner: [ClassOrPackageDataWrapper.Class](../../arrow.common.utils/-class-or-package-data-wrapper/-class/index.md), executableElement: [ExecutableElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ExecutableElement.html)): [Func](../../arrow.meta.ast/-func/index.md) |

## Properties

| Name | Summary |
|---|---|
| [descriptor](index.md#-645837508%2FProperties%2F-35121544) | [jvm]<br>open val [ArrayType](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/type/ArrayType.html).[descriptor](index.md#-645837508%2FProperties%2F-35121544): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [descriptor](index.md#-2070878313%2FProperties%2F-35121544) | [jvm]<br>open val [ExecutableType](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/type/ExecutableType.html).[descriptor](index.md#-2070878313%2FProperties%2F-35121544): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [descriptor](index.md#1102730252%2FProperties%2F-35121544) | [jvm]<br>open val [TypeMirror](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/type/TypeMirror.html).[descriptor](index.md#1102730252%2FProperties%2F-35121544): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [descriptor](index.md#-240230391%2FProperties%2F-35121544) | [jvm]<br>open val [TypeVariable](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/type/TypeVariable.html).[descriptor](index.md#-240230391%2FProperties%2F-35121544): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [descriptor](index.md#2105374311%2FProperties%2F-35121544) | [jvm]<br>open val [WildcardType](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/type/WildcardType.html).[descriptor](index.md#2105374311%2FProperties%2F-35121544): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [elementUtils](index.md#353266973%2FProperties%2F-35121544) | [jvm]<br>open val [elementUtils](index.md#353266973%2FProperties%2F-35121544): [Elements](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/util/Elements.html) |
| [filer](index.md#-575129390%2FProperties%2F-35121544) | [jvm]<br>open val [filer](index.md#-575129390%2FProperties%2F-35121544): [Filer](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/Filer.html) |
| [generatedDir](index.md#-2018801820%2FProperties%2F-35121544) | [jvm]<br>val [generatedDir](index.md#-2018801820%2FProperties%2F-35121544): [File](https://docs.oracle.com/javase/8/docs/api/java/io/File.html)? |
| [hasNoCompanion](../../arrow.common.utils/-processor-utils/has-no-companion.md) | [jvm]<br>open val [Element](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/Element.html).[hasNoCompanion](../../arrow.common.utils/-processor-utils/has-no-companion.md): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [jvmMethodSignature](index.md#2118350669%2FProperties%2F-35121544) | [jvm]<br>open val [ExecutableElement](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ExecutableElement.html).[jvmMethodSignature](index.md#2118350669%2FProperties%2F-35121544): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [locale](index.md#256813368%2FProperties%2F-35121544) | [jvm]<br>open val [locale](index.md#256813368%2FProperties%2F-35121544): [Locale](https://docs.oracle.com/javase/8/docs/api/java/util/Locale.html) |
| [messager](index.md#-1623267801%2FProperties%2F-35121544) | [jvm]<br>open val [messager](index.md#-1623267801%2FProperties%2F-35121544): [Messager](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/Messager.html) |
| [options](index.md#295592682%2FProperties%2F-35121544) | [jvm]<br>open val [options](index.md#295592682%2FProperties%2F-35121544): [Map](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt; |
| [processingEnv](index.md#1453999710%2FProperties%2F-35121544) | [jvm]<br>open override val [processingEnv](index.md#1453999710%2FProperties%2F-35121544): [ProcessingEnvironment](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/ProcessingEnvironment.html) |
| [processingEnv](index.md#-1049675977%2FProperties%2F-35121544) | [jvm]<br>val [processingEnv](index.md#-1049675977%2FProperties%2F-35121544): [ProcessingEnvironment](https://docs.oracle.com/javase/8/docs/api/javax/annotation/processing/ProcessingEnvironment.html) |
| [sourceVersion](index.md#178597355%2FProperties%2F-35121544) | [jvm]<br>open val [sourceVersion](index.md#178597355%2FProperties%2F-35121544): [SourceVersion](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/SourceVersion.html) |
| [typeUtils](index.md#-440752303%2FProperties%2F-35121544) | [jvm]<br>open val [typeUtils](index.md#-440752303%2FProperties%2F-35121544): [Types](https://docs.oracle.com/javase/8/docs/api/javax/lang/model/util/Types.html) |