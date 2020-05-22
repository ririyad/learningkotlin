# learningkotlin
Notes while learning kotlin

> _if I don't get introduced any term by term of writing, I will add '(?)'_

## Basic Types

- In Kotlin, everything is an object **type** in the sense that we can call member functions and properties on any variable.
- Basic Types
  - number (Integer [type(bit)]: [Byte(8), Short(16), Int(32), Long(64)] Floating point: [Float(32), Double(64)])
  - characters
  - booleans
  - arrays
  - strings
- We can use underscore for numeric literals:  
 ```kotlin 
      val oneMillion = 1_000_000
```

## OOP
- `class` can be empty. In that case `{}` can be omitted. Example: `class Empty`
- `class` has one primary constructor (which cannont contain any code) and one or more secondary constructors
- The primary constructor is the part of the class header. For example: 
```kotlin
 class Employee constructor(firstName: String) {...}
 ```
 - The `constructor` keyword can be omitted if the primary constrcutor has no annotations or visibility modifiers.
 
 ## Input Output
 
 **Scenario 1: Based on the number of testcase take 2 inputs from console and print the sum of them**
 
 ```kotlin
 val testCase = readLine()!!.toInt()
 
 for(i in 1..testCase) {
   val(a, b) = readLine()!!.split(" ").map{ it.toInt() }
   println(a+b)
 }
 ```
