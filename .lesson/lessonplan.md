# Lesson 6: If statements (Control Flow){}

<p>&nbsp;</p>

<p dir="ltr"><strong><img src="https://lh6.googleusercontent.com/gMin275RlFfjiQjqYOL3oRqod6RpruSL99DcjGpTKbrpvzlum0rrk0xFC_eQVhVyJjPSjS-n9vmKcB60PNDL0AmHwykHcd4EkBSrk2-r7D4cIa0hIzXk5OGduZUhlRrcz4v1UmDK" style="height:170px; width:297px" /></strong></p>

<p>&nbsp;</p>

<h2 dir="ltr"><strong>Overview</strong></h2>

<p dir="ltr"><strong>Lesson 5 will venture&nbsp;beyond&nbsp;basic variables, types, and mathematical operations.&nbsp; We will be jumping directly into an activity as well as a brand new concepts.&nbsp; Students will:&nbsp;</strong></p>

<ul>
	<li dir="ltr">
	<p dir="ltr"><strong>Learn about using logical and comparison operators in control flow statements</strong></p>
	</li>
	<li dir="ltr">
	<p dir="ltr"><strong>Learn the syntax for <em>if</em> statements</strong></p>
	</li>
	<li dir="ltr">
	<p dir="ltr"><strong>Learn the importance of conditional statements</strong></p>
	</li>
</ul>

<p>&nbsp;</p>

<h2 dir="ltr"><strong>Purpose</strong></h2>

<p dir="ltr"><strong>In Unit 1, we discussed declarations and usable data types in Javascript, all of which are necessary for utilizing if statements properly within app development.&nbsp; <em>If</em> statements provide internal logic within a computer program so that&nbsp;the computer can make decisions based upon the data presented.&nbsp; <em>If</em> statements can be a challenging concept to digest at first.&nbsp; When learning this topic, many students&nbsp;tend to overcomplicate the simplistic nature of <em>if</em> statements.&nbsp; <em>If</em> statements simply are statements that can be evaluated as either being true or false. &nbsp;They&nbsp;can be long or short as long as they&nbsp;can be logically evaluated as being either true or false.&nbsp;&nbsp;</strong></p>

<p>&nbsp;</p>

## Resources
* <a href="https://docs.google.com/presentation/d/1qyqBGuNqd8Waw6KqyHG-oDdGSwlUUTS7co_0gkNcdQg/edit?usp=sharing">If Statement slides</a>

<h2 dir="ltr"><strong>Agenda</strong></h2>

<p dir="ltr"><strong>Getting started (10 mins)</strong></p>

<p dir="ltr"><strong><em>If</em> statement introduction (15 mins)</strong></p>

<p dir="ltr"><strong><a href="https://docs.google.com/presentation/d/1qyqBGuNqd8Waw6KqyHG-oDdGSwlUUTS7co_0gkNcdQg/edit?usp=sharing">if statements slides</a></strong></p>

<p dir="ltr"><strong>Activity (25 mins)</strong></p>

<p dir="ltr"><strong>Wrap up (10 mins)</strong></p>

<p>&nbsp;</p>

<h1 dir="ltr"><strong>Teaching Guide</strong></h1>

<h2 dir="ltr"><strong>Getting Started (10 mins)</strong></h2>

<p dir="ltr"><strong>Remarks</strong></p>

<ul>
	<li dir="ltr">
	<p dir="ltr"><strong>This unit will focus on control flow within Javascript.</strong></p>
	</li>
	<li dir="ltr">
	<p dir="ltr"><strong>Control flow is one of the most commonly used concepts in programming due to its effective way of providing&nbsp;your computer with logical decision making.</strong></p>
	</li>
	<li dir="ltr">
	<p dir="ltr"><strong>Let's go over the basics of <em>if</em> statements with a few visual aids and live examples.&nbsp;&nbsp;</strong></p>
	</li>
</ul>

<p>&nbsp;</p>

<p dir="ltr"><strong>(Refer to slide show for if statements presentation.)</strong></p>

<p>&nbsp;</p>

<h1><a href="https://docs.google.com/presentation/d/1qyqBGuNqd8Waw6KqyHG-oDdGSwlUUTS7co_0gkNcdQg/edit?usp=sharing"><strong>If Statement Slides</strong></a></h1>

</p>

# If Statement Script 

## If Statement Theory (slide 3)
If statements are used to make logical decisions within your Javascript application.
As in life, different scenarios require different methods of approach or outcomes. 

If statements are the core of your applications **logic**.  The ability for your program to make decisions based on what it sees is contingent on a programmers ability to write if statements effectively.

## If Statement Syntax (slide 4)
If statement syntax can be broken down into three different pieces.
* The if keyword
* Parenthesis for conditional statements
* Code block that performs an action if the statement is true.

```javascript
// Keyword       Parenthesis         Codeblock
     if          (condition)             {}
```
The *if* **keyword** signals to javascript to expect an if statement in its entirity after this is written.  Its similar to declaring a variable with any of the *keywords* such as ***let***.  The **condition** is what is being evaluated to either true or false.  While the **code block** is the code that contains the action desired from the developer.  

## If statement example (slide 5)

This example is an evaluation of a string.  On the first line we create a *string* variable called **name** and we give it a value of *"Drake"*.  On the next line is where our if statement performs a simple evaluation using a ***comparison operator***.  Triple equals will evaluate for *equal value & equal type*.  We highly recommend using triple equals in most equivalency comparisons.  It will cause less errors within development in the future.  

## Variable life span in if statements (slide 6)
When creating variables inside of *if statements* their life span only last while the if statement is active.  Meaning once the last line of the **codeblock** is read the variable will not exist.  If the intention is to create a variable that is remembered throughout the program then be sure to create it outside of if statements.

## Nest if statements (slide 7)
If statements can be placed inside of if statements as seen in this slide.  Here is a deeper example that can be understood.

``` javascript 
let weather = "sunny";
let direction = "north";
let destination = "New York";

if(weather === "sunny"){
  if(direction === "north"){
    if(destination === "New York"){console.log("Lets head to New York today since it is nice outside";)}
  }
}
```
The above example should *console.log()* ***"Lets head to New York today since it is nice outside"***.  This occurs because all of our conditions in this scenario evaluate to **true**.  If *"weather"* equals *"sunny"* and if *direction* equals *north* and if *"destination"* equals *"New York"*.  Please take note of the syntax and how the curly brackets all have an opening and closing set and everything that relies on the statement before is inside of said brackets.

## What are conditions
Conditions are statements comprised of variables, operators, and values to which evaluate to true or false.
Conditions can be a single variable, or they can be complex logical statements that use a myriad of operators to evaluate a condition.  Here is a few examples of conditions that belong within the parenthesis
``` javascript
6 < 7  // true
hello !== "hello" // true

// here is how those two conditional statements above will look in if statement syntax
if(6 < 7){...}
if(hello !== "hello"){...}
```
Each of the conditions above is simply using the correct operator in order to complete a statement.  *6 is less than 7* <br>**or** <br> *hello does not equal "hello"*. <br>
The statements are meant to be read similar to how you would speak english.  The only difficulty in putting them together is remembering syntax.  


<h2 dir="ltr"><strong>Activity (25 mins)</strong></h2>

Alice and bob is an exercise that is about recognizing specific names in the forms of strings.  Students should be sure to specifically look for *"Alice"* and *"Bob"* and greet them according to specifications provided by the assignment.

<p dir="ltr">&nbsp;</p>

<p dir="ltr"><strong>&nbsp;</strong></p>

<p>&nbsp;</p>

<h2 dir="ltr"><strong>Wrap Up (10 mins)</strong></h2>

<p dir="ltr"><strong>Review the assignment with the class while having a simultaneous discussion on how <em>if</em> statements make computer programming more efficient.&nbsp;&nbsp;</strong></p>

<p>&nbsp;</p>

<h3 dir="ltr"><strong>Discussion:</strong></h3>

<ul>
	<li dir="ltr">
	<p dir="ltr"><strong>What are some things about <em>if</em> statements that you found difficult?</strong></p>
	</li>
	<li dir="ltr">
	<p dir="ltr"><strong>How do you feel <em>if</em> statements can make programming easier and more efficient?</strong></p>
	</li>
</ul>

<p>&nbsp;</p>

<p dir="ltr"><strong>&nbsp;Be sure to allow students to express their understandings and/or what more they need to learn&nbsp;from this Lesson or the assignment.</strong></p>

<p><br />
&nbsp;</p>

<h1>&nbsp;</h1>

<p>&nbsp;</p>