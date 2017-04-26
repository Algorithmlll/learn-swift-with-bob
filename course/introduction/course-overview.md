# Course Overview
Welcome to Learn Swift with Bob. You've made the right choice. You won't regret the decision you've made to embark the journey with me. Before you and I jumping into the lessons, let us go through the prerequisites, table of content, and course expectation.

## Prerequisites
This course is designed for Swift intermediate. So, I won't cover the basics. Please visit learnSwiftwithBob.com and go to prerequisites. You will find a list of items you are expected to know. There is a YouTube video for each concept, so if you ever get stuck, you can always learn and come back.

#### Variables and Constants
```swift
let imuttableName = "Bob"
var muttableName = "Bobby"

imuttableName = "SangJoon" // Error
```

[Variable vs Constants](https://www.youtube.com/watch?v=W8l-Kt_aKNo&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx&index=1)

#### Conditional Statement
```swift
if isBobHansome {
  print("He good")
} else {
  print("That's okay")
}
```

[Conditional Statement](https://www.youtube.com/watch?v=ayuB4HChkI0&index=2&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx)

#### Array and Dictionary
```swift
let countries = ["S.Korea", "USA", "Vietnam", "Malaysia"]
let info = ["Name": "Bob", "Age": "20"]
```

[Array and Dictionary](https://www.youtube.com/watch?v=yfFkj_8c70o&index=3&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx)

#### For-In Loops
```swift
for _ in 1...100 {
  print("Repeat")
}

// "Repeat"
// "Repeat"
// ...
```

[For-In Loop](https://www.youtube.com/watch?v=bPrdNIEoZio&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx&index=4)

#### Switch Statement
```swift
switch number {
case 1...10 :
  print("Your number is between 1 to 10")
default:
  print("I don't know")
}
```

#### Function
```swift
func returnName() -> String {
  return "Bob the Developer"
}
```

[Function](https://www.youtube.com/watch?v=mvteZcbFRbA&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx&index=6)


#### Intro to Enums
```swift
enum Race: String {
  case asian
  case white
  case black
  case hispanic
}

Race.asian.rawValue // "asian"
```

[Basic Enum](https://www.youtube.com/watch?v=DHCgaQ5GeR4&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx&index=8)


#### Object Oriented Programming
You should be familiar with initialization, property, method, and inheritance

```swift
 class Human {
   let name: String

   init(enterName: String) {
     name = enterName
   }

   func sayName() {
     print("Hi, I'm \(name)")
   }
 }
```

[What is Object Oriented Programming](https://www.youtube.com/watch?v=orvmHi498YI&index=9&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx)

[Inheritance](https://www.youtube.com/watch?v=YtA1b7dX_ZE&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx&index=10)

[Initialization](https://www.youtube.com/watch?v=Jejtrj9Xfpk&index=11&list=PL8btZwalbjYlRZh8Q1VK80Ly0YsZ7PZxx)


## Table of Content
Go to learnSwiftwithBob.com and click Table of Content. There are 8 chapters in this course. From Chapter 1 to 4, you will get a firm understanding of both Functional, and protocol, and Object Oriented Programming. In Chapter 5, you will fully understand how objects are created and removed. In Chapter 6 and 7, you will learn how to create value oriented swift code along with protocol generics and enums. In the last Chapter, you will learn a various advanced and hidden tips and secrets about the Swift programming languages. 

## Course Expectation
Based on the Stack Overflow survey in 2016, Swift is considered as the second most loved language out of thousands. However, don't let its readability and hype fool you. It's a complex language inspired by many programming languages out there. In fact, you will suffer, and I want it that way. Let me explain.

### Be Skeptical
I’m a biased human being. I hope you do not trust me all the way. If you spot any practices that raise your eyebrows, make sure challenge me and come up with a better solution. Although I try to prevent that from happening through doing my homework, I encourage you to think outside of the box.

### Be Proactive
You might have seen those red error messages on the left side. I expect you to figure out and search what the issue is. Copy and paste the error message on Google. Ask me questions. Do whatever it takes. Do not move on without knowing the cause and how you could prevent them from occurring.
I mentioned that learning is done by you, not me. I’m here to teach you how to catch fish. I’m going to show you how to use nets and fish rods. After this course, you are expected to use those tools on your own. You might cut yourself through sharp edges, but it's just a part of your learning journey and becoming a stronger version of yourself.

## Ideal Learning Stage
| Step | Detail |
|: --- :| --- |
| The Why | Each lesson should flow like a story. In the beginning, I start off with a problem statement. It consists of doubts and questions I personally encountered. For example, I would ask, what's the purpose of using optionals? A problem statement organically leads to why we learn such materials and features
| Application | After having gone through the specific problem statement by showing new features and how to use them, I present how it applies to real-life situations.
| Resources | I attach additional resources for you to study more. You may go further on your own.
| Visualization | It's your turn. I don't believe in practice problems. We no longer live in a world where there are fixed answers. You visualize how the feature you've learned can be applicable for your future endeavor. Albert Einstein said, "Imagination is more important than knowledge". Practice problems turn you into a machine. We have more than enough in 2017, by the current education system.
| Test |  It's time to put your visualization into practice. You should fail. That's good. You are trying something new. "Failure is an option here. If things are not failing, you are not innovating enough" - Elon Musk

#### Source code
[0002_Prerequisites](https://www.dropbox.com/sh/33thop7ornp9u90/AACA-JPFoW3ie4EAW56-WZH2a?dl=0)
