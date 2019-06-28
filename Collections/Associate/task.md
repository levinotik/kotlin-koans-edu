## Associate

Read about [association](https://kotlinlang.org/docs/reference/collection-transformations.html#association).
Implement the following functions using 
[`associateBy`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/associate.html),
[`associateWith`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/associate-with.html)
and [`associate`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/associate-by.html):

- building a map from customer name to customer
- building a map from customer to their city 
- building a map from customer name to their city

```kotlin
val list = listOf("abc", "cdef")

list.associateBy { it.first() } == 
        mapOf('a' to "abc", 'c' to "cdef")

list.associateWith { it.length } == 
        mapOf("abc" to 3, "cdef" to 4)

list.associate { it.first() to it.length } == 
        mapOf('a' to 3, 'c' to 4)
```