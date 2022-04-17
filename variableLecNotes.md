# Variables
## What is a "variable"
A variable is a bucket

![](https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/google/313/bucket_1faa3.png)

---
A variable is a bucket _with an address_.

![](https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/google/313/bucket_1faa3.png)

---
If we want to be totally precise, a variable is just an address, but I think the bucket part is a better metaphor. 

---

Let's look at some code

```cs
// This is a comment
int a;
```

If you notice the first line we used a pair of slashes to define a comment. Comments are parts of the document that are ignored by the complier. 

> Why might we want to write stuff that is ignored by the complier?

--- 

```cs
// This is a comment
int a;
```

On the second line of code we are declaring a variable. In this case the `int` indicates it is an _'integer'_ (a whole number, no decimals) and we are giving it the name `a`.

---

You will also notice that there is a semi colon a the end. In C# commands are terminated with semicolons. Think of it like the period at the end of a sentence. 

Lets say we want to do something with our variable. How about we try printing it's contents to the console: 

```cs
int a;
Debug.Log(a);

// Result
// 0
```

If you remember, a variable is a bucket. It holds stuff. When we use the name of the bucket (the variable name) we are telling the complier to take whatever is in the bucket and use it there. 
In this case we are telling it to print the contents to of that variable to the console, and it prints out a zero. 

Where did that zero come from? Where possible, when you declare a variable it will be assigned a default value. In the case of most numbers the default value is `0`. So when we print it to the console, we get 0.

---

If we want to store any _other value_ in the variable we need to assign it. 

```cs 
int a;
a = 6;

// Result
// 6
```
Here we declare our variable `a` and then we assign it the value of 6. 

To save some typing we can combine the declaration and the assignment into one line. 
```cs 
int a = 6;

// Result
// 6
```

It's not a problem to assign the default value to a variable. In fact some times it is preferred to do so just to make it easier to follow what the code is doing. 

```cs
int a = 0;
```

---

What else can we do with variables? 

We can perform a number of mathematical operations:

```cs
int a = 0;
int b = a + 1;
// a is 0
// b is 1

b = a - 2;
// a is 0
// b is -2

int c = b * 3;
// c is -6

int d = c * b;
// d is 12

int e = d / 4;
//e is 3
```

The equal (assignment) operator takes whatever is on the left side and sets it equal to the whatever is on the right side. If you have take algebra, most of these symbols should be pretty straightforward. 
