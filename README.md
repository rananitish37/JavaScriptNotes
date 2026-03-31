# Intro
Everything in javascript happens inside **execution context**

Execution context is like a big box which has two component.
Memory component ( Variable environment): kind of environment where all the variable present in key value pair.

Another is code where actual code present.
[[Execution context]]

JavaScript is a synchronous Single threaded language:
Single threaded means: Javascript can execute one line at a time.
Synchronous means: At particular order

{**Java script can execute single line at a time at a specific order**}


# Execution (Execution Context)
Call stack maintain the order of execution of Execution Context.

Call Stack: Execution Context Stack, Program Stack, Control Stack, Runtime Stack, Machine Stack.


```
var n = 3;
function square(num){
	var ans = num * num;
	return ans;
}

var square1 = square(n);
var square2 = square(4);
```

See the execution in : [[ExecutionDemo]]
