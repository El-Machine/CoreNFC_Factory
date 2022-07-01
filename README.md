

![Pipe](logo.png?raw=true "Title")

### It’s possible to incapsulate whole data receiving process into one symbol?

Declarate variable  
```swift
var a: Foo
```
Add one symbol 
```swift
*(a as Foo), Foo.self^, etc...
```
Receive data
```swift
a != nil
``` 

### Pipe is attempt to find an answer

>In Unix-like computer operating systems, a [pipeline](https://en.wikipedia.org/wiki/Pipeline_(Unix)) is a mechanism for inter-process communication using message passing. A pipeline is a set of processes chained together by their standard streams, so that the output text of each process (stdout) is passed directly as input (stdin) to the next one. The second process is started as the first process is still executing, and they are executed concurrently.

```bash
command1 | command2 | command3

ls -l | grep key | less
```

### Usage

```swift
//Anything from Something
let anything: Anything = something|

let i: Int = float|
let string: String = data|

let front: UIColor = 0x554292|
let back: UIColor? = "#554292"|

//Anything from Nothing
|{ (anything: Anything) in
🧙🏼
}

|{ (location: CLLocation) in 

}

|{ (data: CMPedometerData) in 

}

|{ (peripheral: CBPeripheral) in 

}

UIWindow.keyboardWillShowNotification | { (n: Notification) in
            
}

```
### Idea
Just imagine that you have a pipe and look into it from your side  
You don't know what is already in pipe or what will happens on another side of pipe   
Simply get objects that you need on your side

### Сoncept

Pipe started from idea about receiving anything in most efficient and fast way  
Just add one sign to completion handler and start receiving the result  
Current implementation is not final solution, but main idea

You ideas, comments, contribution are welcome  
Main course is to add some new Pipable extensions for other types