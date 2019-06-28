## For loop

Kotlin [for loop](http://kotlinlang.org/docs/reference/control-flow.html#for-loops)
can iterate through any object if the corresponding `iterator` member or extension function is available.

Make the class `DateRange` implement [`Iterable<MyDate>`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/kotlin.-iterable/),
so that it could be iterated over.

Use [object expression](http://kotlinlang.org/docs/reference/object-declarations.html)
which plays the same role in Kotlin as anonymous class in Java. 
Also, use the function `MyDate.nextDay()` defined in `DateUtil.kt`.