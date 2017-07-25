## Project Name:  Income Tax Calculator Application

### Course Title:
LIS 2360:  Web Application Development

### Assignment Date:  
July 24 , 2017.

### Student Name:  
Sharon Ballinger.

### Project Description:
Introduction to JavaScript, by using arrays, loops, functions and conditional statements.

### View Project:
https://sharonballinger.github.io/lesson5_javascript2/

### Lessons Learned in the Assignment:

#### **1. What is a _Conditional Statement_.**
Conditional statements are used to perform/ask a question and to receive an action/answer – the answer will be either true or false.
Coding a conditional statement is created by writing an expression with the use of relational operators.
|Operator|Description|Use of operator|
|---|---|---|
|==|Equal|First name == "Sharon" (answer is true)|
|!=|Not equal|Summer != cold (answer is true)|
|<|Less than| 1 < 5 (true)|
|<=|Less than/equal|Drinking age in Europe is <= 18 (false)|
|>|Greater than|25 > 20 (true)|
|>=|Greater than/equal|Drinking age in Europe is >= 18 (true)|

The above conditional statements argue only one statement with the answer being true or false. Adding logical operators: `&&` AND; `||` OR; `!` NOT, enables more than one expression to be strung together and creates a compound conditional expression. To make the conditional statements an active expression, Javascript has four different options: 'if', 'else', 'else if' or switch (See below _Composing a conditional Statement_).


#### **2. Composing a _Conditional Statement_.**
Javascript has four different "action" words to help create a Conditional Statement:
- **if** is used to decribe the code as **true**.
- **else** is used to describe the same code as **false**.
- **else if** is used when the first code returns a *false*, the *if* creates a new statement.
- **switch** is used when there are many different answers to the statement.
**if**
```
if (today = Monday) {
    greeting = "Happy Monday"
}
```
The Condiitonal Statement is true, today is Monday and we are greeted with: Monday Blues

**else**
```
if (today = Monday) {
    greeting = "Monday Blues"
} else {
    greeting = "Glad it isn't Monday!"
}
```
Today isn't Monday so the Condiitonal Statement is false, we are greeted with: Glad it isn't Monday!

**else if**
```
if (today = Monday) {
    greeting = "Monday Blues"
} else if (today is Saturday || Sunday) {
    greeting = "Welcome to the weekend"
} else {
    greeting = "I can't wait for the weekend to begin"
}
```
If today is **Monday**, the greeting is **"Monday Blues"**, if the day is a **Saturday** or a **Sunday**, the greeting is **"Welcome to the weekend"**, if it is neither of these, the greeting is **"I can't wait for the weekend to begin"**.

**switch**
```
var color = prompt ("What is your favorite color of the rainbow?", "Type your favorite color");

switch (color) {
    case 'red':
        text = "Red is an energizing and powerful color of the rainbow";
        break;
    case 'orange':
        console.log("Orange helps to keep us energized and is a happy color of the rainbow");
        break;
    case 'yellow':
        console.log("Yellow is an illuminating color and is the color of fun in the rainbow");
        break;
    case 'green':
        console.log("Green is a harmonious color, it offers balance to the rainbow");
        break;
    case 'blue':
        console.log("Blue is the color of trust, it shows control and direction within the rainbow");
        break;
    case 'indigo':
        console.log("Indigo is the color of structure, without it the rainbow wouldn't be so strong");
        break;
    case 'violet':
        console.log("Violet is the color of imagination, it is the spirit of the rainbow");
        break;
    default:
        console.log("Are you sure you can see a rainbow?")
}
```
There is a pop-up that says: **"What is your favorite color of the rainbow?"**
You answer: **"red"** the new pop-up says: **"What is your favorite color of the rainbow."**

If you put **"teal"** as your answer the pop-up says **"Are you sure you can see a rainbow?"**


#### 3. What are Loops?
Think of a piece of rope and make a loop. Eventually, the ends will cross over one another. What happens if it doesn't cross over; it doesn't create a solid loop. Same thing applies in computer programming code: a loop will continue to execute a statement until a condition is matched. If the condition is unmatched, it keeps going until eventually it crashes the programme. The idea behind loops is to work smarter not harder which equals less coding! 
Three types of loop conditions:
- **for** loops through the code multiple times.
- **for/in** loops through an object.
- **while** loops through the code while something is true.
- **do/while** loops through the code while something is true.


**The _for_ loop**
```
function saySomething() {
    document.write("hi there!");
}

for (var s = 0; s < 10; s++) {
    saySomething();
}
```
The Keyword `"for"` is used, then a starting state of `"s = 0"`, then the stopping state of `"s < 10"` "less than 10" and finally how we increment s by 1 `"s++"`, the say something is called when the statement reaches less than 10.

**The _for/in_ loop**
```
var text = "";
var person = (firstname:"David", lastname:"Beckham", occupation:"sporting superstar");

for (var x in person)
{
    text + text + person(x);
}
```
What will be written is: `David Beckham sporting superstar`.
Instead of writing code multiple times for an object you can simplify the code to loop through it. In the case above all we wrote was: `text + text + person(x)`, it accessed the information **inside** of the `var person` variable.

**The _while_ loop**
```
while(condition) {
    //statements
}
```
The while loop will carry on running until it becomes false. For example it runs and the anwer is true, so it runs again and again until finally it is false. Everytime it runs a loop this is known as an iteration. There will be multiple iterations until the false condition is met. It will either carry on running or stop. What happens if it keeps looping and looping and there is no false statement met? An infinit loop while occur and more than liking shut down your computer. To counteract this the `(condition)` needs to be declared as a variable. Below shows `x=1`.

```
var x=1;              // my counter is starting at 1
while(x <= 20) {      // while 'x' is less than or equal to 20
    document.write("Hello there" "+ x +"); // the statement is "Hello there"
x++;                  // x plus 1

}
```
The iteration will stop at 20, because 21 will result false.
The result will be `Hello there 1` through `Hello there 20` on separate lines.

**The _do/while_ loop**
```
do{
    // statements
} while(condition);
```
The _do/while_ loop  is similar to the _while_ loop. If your loop creates a false iteration straight away but you would prefer the loop to run at least once before it stops. The `do` runs the following statements then it runs the condition until it become false.
```  
var x=21;              // my counter is starting at 21
    
do{
    document.write("This is my attempt "+ x +"<br/>");
x++;                   // x plus 1
}while(x <= 20);       // x is less than or equal to 20
```
21 is greater than 20 so the loop is false. As there is a do/while statement to runs the code once and stops at `This is my attempt 21`.
