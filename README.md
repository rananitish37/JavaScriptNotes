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


# Hoisting
Hoisting is a phenomena in javascript by which you can access variable even before we initialised and put some value in it.

1. When we declare a variable(Using var) before trying access them it will print undefined
2. Undefined in javascript not similar as not define as in other languages it is basically a datatype we can say which is assigned to the var when not data is assigned in first phage of the execution.
3. The arrow function will look like behaving the same as var variables so during first phase arrow function will also have the undefined initially.
4. But if the function is not arrow if it is declare with function keyword then at first phage itself it will store the entire function body in memory.

