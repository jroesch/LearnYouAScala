This is a companion work to a talk I was giving on Scala, and all examples are provided in the source tree. 

# Introduction
>Scala is a general purpose programming language designed to express common programming patterns in a concise, elegant, and type-safe way. It smoothly integrates features of object-oriented and functional languages. It is also fully interoperable with Java.

- [Scala's Webpage](www.scala-lang.org)

## References 
Scala's reference's come in two flavors, mutable and immutable. The keywords ```var``` and ```val``` define these respectively. Variables in Scala are declared and defined at the same time. The only difference between the two is the mutablitity of the references themselves. ```var``` can be re-assigned to while ```val``` cannot.
```Scala
/**
 * String Objects are immutable themselves we are just mutating the references here.
 */
var a: String = "hello"
val b: String = "world"
// we can reassign to a
a += b
// but not to b
b = a + b
```

## Literals 
Scala formation of literals is nearly identical to Java's, in fact String is just an alias for java.lang.String.
The biggest difference is that we can treat everything in Scala as an object, unlike Java where there are primatives, aka value types, Integers, Doubles, Characters, Bytes, Booleans.\

```Scala 
// Integer Literals
val hexLiteral: Int = 0xFF
val octalLiteral: Int = 0377
val decimalLiteral: Int = 255

// String Literal
val stringLiteral: String = ""
```
## 