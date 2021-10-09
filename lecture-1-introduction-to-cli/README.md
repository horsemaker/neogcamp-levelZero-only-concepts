# Introduction to CLI
### What is CLI ?<br />
- CLI stands for Command Line Interface<br />
- Command Line Interface is a text-based interface which processes the commands of a computer program in the form of lines of text to   perform functions and responds back in the same way.

## Concept no 1: JavaScript and NodeJS
### JavaScript 
- A text-based programming language which executes on a browser, allows to make webpages interactive.
JavaScript is a programming language, which runs in browser.
### NodeJS
- Node.js is an interpreter or running environment for JavaScript

### JavaScript can run in a browser as well as in CLI only if NodeJs runtime environment is installed.

Tools we can use for JavaScript and NodeJS
- [repl.it](https://replit.com/)
  - What is a repl?<br />
   repl stands for read-evaluate-print-loop <br />
   Replit is a simple yet powerful online IDE, Editor, Compiler, Interpreter, and REPL. Code, compile, run, and host in 50+               programming languages.

- Any Browser 
   - JavaScript can run inside nearly all modern web browser

## Getting started with JavaScript

### 1. To print the output
- To print a statement in both browser or in CLI<br />
<code>console.log(“statement”);</code>

### 2. To get the input from the user
- In browser<br />
<code>prompt(“enter your name”);</code><br />
Returns the user's input in console
- In NodeJS/ CLI app<br />
In NodeJS/ CLI we need something to get the input, for that purpose we use [<code>readline-sync</code>](https://www.npmjs.com/package/readline-sync) <br />
    - To get <code> readline-sync</code>, first we need to get <code>npm</code> <br /><br />
    - [What is <code>npm</code>?](https://nodejs.org/en/knowledge/getting-started/npm/what-is-npm/#:~:text=npm%20is%20two%20things%3A%20first,version%20management%2C%20and%20dependency%20management.) <br />
    An online repository for the publishing of open-source Node.js projects and it is a command-line utility for interacting with said repository that aids in package installations, version management, and dependency management.<br /><br />
    Steps to get <code>readline-sync</code> <br />
    1. First install and setup nodejs from [nodejs.org](https://nodejs.org/en/), <code>npm</code> will be included in this as well.
    2. Open Command Prompt to check whether the installations were success or not by running the command <br />
    <code>node -v</code>
    it should give the version of nodejs<br /> 
        >v10.16.3<br />
        >
        Similarly, <br />
        <code>npm -v</code>
    it should give the version of npm<br /> 
        >v6.9.0<br />
        >
    3. Install <code>readline-sync</code> by running command in Command Prompt   
    <code>npm install readline-sync</code><br /><br />
    
    - **<code>readline-sync</code> is a npm-library**
    
   - What is a library?<br />
   It is a collection of pieces of pre-defined/ already written codes which can be used as it is in bigger programs.

   - After installing required packages, the readlinSync will get added as a <code>dependency</code>.
   - What do we mean by a <code>dependency</code>?<br/>
   A dependency in programming is an essential functionality, library or piece of code that's essential for a different part of the code to work. For example, a specific library that a given line of code depends on.
   
   - How to declare <code>readlineSync</code>?<br/>
   Syntax : <code>var readlineSync = require(“readline-sync”);</code>
   - readlineSync can be used in 3 ways : 
      -  <code>readlineSync.question('question?')</code><br />
            In this case, the users are prompted to type the answer manually.
      -  <code>readlineSync.keyInYN('question?')</code><br />
      In this case,the users are prompted to type their answer as <code>y</code> ( returns <code>true</code> ) or <code>n</code> ( returns <code>false</code> ) only.
      -  <code>readlineSync.keyInSelect(answerSetArray, 'question?')</code><br />
            In this case, along with the question, the mentioned **answerSetArray**'s elements would be displayed as multiple choices for the given question.<br /> The users are prompted to type the index ( which will be mentioned alongside the choices ) of the correct answer.
      



