#### Reference: [Functional Swift](https://www.objc.io/books/functional-swift/) by [Chris Eidhof](https://twitter.com/chriseidhof)

## What is functional programming in Swift
 * **Modularity:** Rather than a sequence of assignments and method calls, FR emphasizes creating smaller pieces. 
 * **A Careful Treatment of Mutable State:** FR is half-jokingly 'value-oriented programming'. Unlike OOP with encapsulated state, FR is all about free of mutable state or other side effects. 
 * **Types:** A functional program makes careful use of *types*

Functions in Swift are *first-class values*. Functions can be passed to other functions. 

```swift
func add1(_x: Int, _y: Int) -> Int {
 return x + y
}

```
The code above is identical to the bottom 

```swift
func add2(_x: Int) -> ((Int) -> Int) {
 return { y in x + y }
}

add2(1)(2) // 3

```
`add2` is said to be the *curried* version of `add1`. Why is it so interesting? 

## Introducting Generics
Suppose we need to write a function that, given an array of integers, computes a new array, where every integer in the original array has been incremented by one. 

```swift
func increment(array: [Int]) -> [Int] { var result: [Int] = []
 for x in array {
  result.append(x + 1) 
  }
  return result 
}
```

Now, suppose we need a function that computes a new array, where every element in the argument array has been doubled, 

```swift
func double(array: [Int]) -> [Int]) {
 var result: [Int] = []
 for x in array {
  result.append(x * 2)
 }
 return result 
}
```

Both of the two examples above share a lot of code. 

```swift
func compute(array: [Int], transform: (Int) -> Int) -> [Int] { 
 var result: [Int] = []
 for x in array {
  result.append(transform(x)) }
 return result 
}
```

Once again, the function isn't that interesting. It has to do with Int stuff only. 

```swift
func double2(array: [Int]) -> [Int] { return compute(array: array) { $0 * 2 }
}
```

Introducing Filter

```swift
extension Array {
 func flter(_ includeElement: (Element) -> Bool) -> [Element] {
  var result: [Element] = []
  for x in self where includeElement(x) {
   result.append(x) 
  }
  return result 
  }
}
```

## Generics vs the Any Type
```swift
 func noOp<T>(_ x: T) -> T {
  return x 
 }
```
or 
```swift
func noOpAny(_x: Any) -> Any {
 return x
}
```
Both noOp and noOpAny will accept any argument. The crucial differnece is what we know about the value being returned. 


## Optional Chaining
```swift
if let person = order.person {
 if let address = person.address {
  if let state = address.state { print("Got a state: \(state)")
  }
 }
}
```















