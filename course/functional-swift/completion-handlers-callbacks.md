# Completion Handlers

## Introduction
Welcome to Lesson 4 of The UIKIt Fundamentals Part 1 Intro to Functional Programming. This is the last lesson. But, this is the important lesson we will talk about in this course. You will definitely see a lot of completion handler blocks when it comes to using APIs such as getting images from Facebook, Instagram, and so on. You will learn what completion handlers is and why we use it in the first place. Enough of said, let's get into the meat and potatoes. However, again, learning completion handlers is challenging. It took weeks for me understand. I could have done an extraordinary job in explaining, but I still expect you feel uncomfortable. Don't worry. We will dive more in Part 2 and Part 3 of this course.

## Problem
I've heard about it. I don't know how to make one

### Usage
  1. Notify the user when download completed
  2. Animation

### Design Handler Block
If you pass `true`, it calls a print statement.
```swift
let handlerBlock: (Bool) -> () = { (isSucess: Bool) in
  if isSucess {
    print("Download has been finished")
  }
}
```
The example below is a shorter way to write a closure block.
```swift
let handlerBlock: (Bool) -> () = {
  if $0 {
    print("Download Completed")
  }
}
```

You may run the closure.
```swift
handlerBlock(true) // "Download has been completed"
```

### Design Function
Create a function that imitates the user downloading an image by calling a `for-in` loop. Once the download has been finished, you may pass `completionHandler(true)` which will run the print statement.

```swift
func downloadAnImage(completionHandler: (Bool) -> ()) {

  for _ in 1...1000 {
    print("Downloading")
  }

  completionHandler(true)
}
```

```swift
downloadAnImage(completionHandler: handlerBlock) // Good
```

#### Pass Closure Directly
```swift
downloadAnImage(completionHandler: { (isSucess: Bool) in
  if isSucess {
    print("Download has been finished")
  }
 }
)
```

#### Use Trailing Closure
```swift
downloadAnImage { (isSucess) in
  if isSucess {
    print("Download has been finished")
  }
}
```

### Source Code
[3006_completion_handlers.playground](https://www.dropbox.com/sh/t47kpcnzuhtgni9/AAA1Yvq52s6XVOFgMLRjOPRka?dl=0)

### Resources

## Conclusion
That's it.
