# Introduction to CLI
### What is **CLI** ?<br />
- CLI stands for **Command Line Interface**<br />
- **Command Line Interface** is a text-based interface that processes the commands of a computer program in the form of lines of text to perform functions and responds in the same way.

## Concept no 1: JavaScript and NodeJS
### JavaScript 
- A text-based programming language which executes on a browser, allows making webpages interactive.
JavaScript is a programming language, which runs in the browser.
### NodeJS
- Node.js is an interpreter or running environment for JavaScript

### JavaScript can run in a browser as well as in CLI only if **NodeJs runtime environment** is installed.

Tools we can use for JavaScript and NodeJS
- [repl.it](https://replit.com/)
  - What is a repl?<br />
   repl stands for **read-evaluate-print-loop**<br />
   Replit is a simple yet powerful online IDE, Editor, Compiler, Interpreter, and REPL. Code, compile, run, and host in 50+               programming languages.

- Any Browser 
   - JavaScript can run inside nearly all modern web browser

## Getting started with JavaScript

### 1. To print the output
- To print a statement in both browser or in CLI<br />
<pre>console.log(“statement”);</pre>

### 2. To get the input from the user
- In browser<br />
<pre>prompt(“enter your name”);</pre><br />
Returns the user's input in console
- In NodeJS/ CLI app<br />
In NodeJS/ CLI we need something to get the input, for that purpose we use [<code>readline-sync</code>](https://www.npmjs.com/package/readline-sync) <br />
    - To get <code> readline-sync</code>, first we need to get <code>npm</code> <br /><br />
    - [What is <code>npm</code>?](https://nodejs.org/en/knowledge/getting-started/npm/what-is-npm/#:~:text=npm%20is%20two%20things%3A%20first,version%20management%2C%20and%20dependency%20management.) <br />
        - npm stands for **node package manager**<br/>
        - It is an online repository for the publishing of open-source Node.js projects and it is a command-line utility for interacting with said repository that aids in package installations, version management, and dependency management.<br /><br />

    Steps to get <code>readline-sync</code> <br />
    1. First install and setup nodejs from [nodejs.org](https://nodejs.org/en/), <code>npm</code> will be included in this as well.
    2. Open Command Prompt to check whether the installations were success or not by running the command <br />
    <pre>node -v</pre>
    it should give the version of nodejs<br /> 
    >v10.16.3<br />
    >
    Similarly, <br />
    <pre>npm -v</pre>
    it should give the version of npm<br /> 
    >v6.9.0<br />
    >
    3. Install <code>readline-sync</code> by running command in Command Prompt   
    <pre>npm install readline-sync</pre><br /><br />
    
    - **<code>readline-sync</code> is a npm-library**
    
   - What is a library?<br />
   It is a collection of pieces of pre-defined/ already written codes which can be used as it is in bigger programs.

   - After installing required packages, the readlineSync will get added as a <code>dependency</code>.
   - What do we mean by a <code>dependency</code>?<br/>
   A dependency in programming is an essential functionality, library, or piece of code that's essential for a different part of the code to work. For example, a specific library that a given line of code depends on.
   
   - How to declare <code>readlineSync</code>?<br/>
   Syntax : <pre>var readlineSync = require(“readline-sync”);
   var userInput = readlineSync.question("question");</pre>
   - readlineSync can be used in 3 ways : 
      -  <code>readlineSync.question('question?')</code><br />
            In this case, the users are prompted to type the answer manually.
      -  <code>readlineSync.keyInYN('question?')</code><br />
      In this case,the users are prompted to type their answer as <code>y</code> ( returns <code>true</code> ) or <code>n</code> ( returns <code>false</code> ) only.
      -  <code>readlineSync.keyInSelect(answerSetArray, 'question?')</code><br />
            In this case, along with the question, the mentioned **answerSetArray**'s elements would be displayed as multiple choices for the given question.<br /> The users are prompted to type the index ( which will be mentioned alongside the choices ) of the correct answer.
      
## Basic concepts     
### 1. Variable
- What is a <code>variable</code>?<br />
It is a placeholder in computer memory, where we store a certain value that we will access in the future via a reference name.
  - There are different types of variables :
     - String
     - Number
     - Boolean and many more
### How to declare a variable ?
-  To declare a variable we can use three keywords .i.e. var, let, and const
    -  Syntax:  
    <pre>var userName = "user"; </pre>
-  When to use var, let, and const?
    1. <code>var</code> <br />
    It can be global/functional scoped and it is used for variables that need to be re-declared and updated.
    2. <code>let</code> <br />
    It is block-scoped and can be updated but not re-declared.
    3. <code>const</code> <br /> 
    It is also block-scoped but it can't be updated or redeclared.
### CamelCase
-  Camelcase is used preferably as naming convention in Javascript.
- Example: <code>userName, getPrice, etc.</code>

### String 
- String can be any text written inside double or single quotes.
- <code>String Concatenation</code>
    - Adding two strings or merging two strings, using the addition sign “ + ” is called string concatenation. 

### 2. Data Structures
A **Data Structure** is a particular way of organizing data in a computer and **Array** is the simplest data structure where each data element can be randomly accessed by using its index number.
- In JavaScript, Arrays are not primitive, they are **Objects**<br />

### Object
- An Object stores the data in form of key-value pairs.
- The values can be accessed by using their respective keys.
- Therefore, these keys act as properties of the object.
- How do we access property?
  - We access property by using *dot* notation
  - Example:<br />
  <pre>var Obj = {key:value};
  console.log(Obj.key);</pre>
  >value
  >
  *Everything in JS is an Object*
  
## Processing 
### Conditional Statements
- Conditional Statements decides whether to run the piece of code or not.<br />
- The very best example is <code>if-else</code><br />
- In <code>if-else</code> block 
    - first the condition is checked
    - if the condition returns <code>true</code> then the piece of code present within the <code>if</code> block executes
    - else if the condition returns <code>false</code> then it will run the code present in the <code>else</code> block
    - Syntax
    <pre>
        if(condition) {
            // if condition true then this block will be executed
            // set of statements
        }
        else {
            // if condition false then this block will be executed
            // set of statements
        }</pre>

### Functions
   - <code>Function</code> is a set of statements that can be used repetitively in one single program just by calling it by its reference name and passing arguments in it.<br/>
   - Function is a repeating piece of the processing unit.<br/>
   - Syntax:
   <pre>
    function functionName(parameterOne, parameterTwo) {
    // processing
    return outputValue;
    }
    </pre>


#### What are Parameters and Arguments?
- **Parameters** are the names of the variables present in the function definition.
- **Arguments** are the real values passed to the function and received by them.


### Control Flow Statements
   - The <code>control flow</code> is the order in which the computer executes statements in a script.<br/>
   - The example we learnt is <code>for loop</code><br />
   - <code>For loop</code> runs the set of statements mentioned/written inside the block, repetitively until the exit condition is met.<br />
   - Syntax: 
<pre> for (intial CONDITION; exit CONDITION; change CONDITION) {
    // code block to be executed
    }</pre>


## Styling     
### Chalk
- [<code>Chalk</code>](https://www.npmjs.com/package/chalk) module in Node.js is the third-party module that is used for styling the format of text and allows us to create our themes in the node.js project.
- To use <code>chalk</code>,module we need to first install it by running the below command line:
<pre> npm install chalk</pre>
- How to use <code>chalk</code>?
<pre>const chalk = require('chalk');    // to get the chalk module</pre>

