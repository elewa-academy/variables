# Variables & Types

The most basic unit of JavaScript is the __variable__. Variables are a way for you the programmer to think about, talk about, and understand what is happening inside the computer.  

This page outlines most of the most important aspects of using variables in JS and provides you with the study skills necessary to explore them on your own using whatever examples or tutorials you prefer. 

The most important take-aways from this page are:
1. Using PythonTutor.com to visualize how JavaScript works behind the scenes.
2. Using sketches on paper to visualize JavaScript runtime behavior.
3. Becoming JavaScript. Learning to step through code as though you were the computer using nothing but pencil & paper.

You will know you have mastered these three skills when you can describe every change that will take place in PythonTutor before clicking the 'forward' button.  These skills aren't very glamorous and will take plenty of work to master, but mastering them now will ensure your success when you encounter more challenging code later on. 

Not taking the time to learn these skills now may feel harmless and probably won't stop you from moving forward for the first few weeks, but you will soon reach a point where not having these skills under your belt will keep you from moving forward.  By then it's too late, you'll need to do some unlearning. 


### Index
* [Learning Objectives](#learning-objectives)
* [Specifications](#specifications)
* [Resources](#resources)

---

## Learning Objectives

__Study Techniques:__
* Stepping through run-time behavior with PythonTutor
* Sketching run-time behavior on paper
* Changelog tracing: what changed with each step?

__JavaScript:__
* Creation & Execution Phases
  * Creation (step 1 in PythonTutor)
  * Execution (every other step)
* Variables: var, let, const
  * Assignment by value
  * Assignment by pointer
  * Reassignment
  * Hoisting behavior
* Data types:
  * Primitive vs Objects  
  * Type Conversions
* Objects (without methods):
  * Dot vs. Bracket access
* Arrays:
  * Basic array methods

__Programming Skillzz:__
* Code life-cycle:
  * Source-time: The code that's written
  * Build-time: JavaScript creation phase
  * Run-time: When JS executes lines one at a time
* Working with primitives:
  * Evaluating operations by hand
  * Evaluating comparisons by hand
* Tracing variables:
  * Creation & hoisting (build-time)
  * Assignment & reassignment
  * Chained assignments
  * Shared references
* Tracing data structures:
  * Source-time values
  * Run-time values
  * Step-by-step changes in value
* Working with nested data structures:
  * Arrays in Arrays
  * Objects in Objects
  * Arrays in Objects
  * Objects in Arrays
* Helpful variable names





[TOP](#variables-&-types)

---

## Specifications

In order to focus on variables, we recommend that you limit your step-throughs & diagrams to samples of code that contain only variable assignments and data structure manipulations (for now).   This means no loops & conditionals (scope) or functions (context) for now.  The diagrams for sketching these language features are more complex and rely on a firm grasp of tracing variables & data structures.

At the beginning you should think of these diagrams as __descriptive__, you are simply redrawing what PythonTutor has displayed on the screen after you press the 'forward' button.  As you practice you should make an effort to avoid looking at the screen whenever you can.  The goal of these exercises is that your diagrams will become __predictive__.  You will know you are ready to move on to scope when you can draw what PythonTutor will display _before_ clicking the 'forward' button.

These diagrams are __change logs__. You won't be drawing everything on the screen for every step, you will only be keeping track of what changes from step to step.  _It should ..._
* _keep track of which step of the program is being executed._
* _indicate the last line executed, the current line being executed, and the next line to be executed._ 
* _describe what is taking place in plain English._  This will capture information that is not directly displayed in the diagram and will make it much harder to just copy what's on the screen.
* _indicate a new variable is declared with a plus sign followed by the name and value of the variable._
* _indicate a variable is modified by showing the old value and the new value._
* _indicate something is written to the console._ You will write the same text in the console box of your sketch.
* _indicate when an object or array is created._ You will indicate this with a plus sign followed by a sketch of the new data structure.
* _indicate when an object or array is modified._ Much like with variables: a new property is indicated with a '+', a removed property is indicated with a '-', and a modified property is indicated by writing the old value and the new value.





[TOP](#variables-&-types)

---

## Resources

__Completed step-through diagrams to study:__

These examples serve two purposes:
1. Teach by example how to sketch JavaScript's execution behavior.
2. Highlight some of the tricky (but very important) features of JS Variables & Types.   

These examples seem simple on the surface, but are very important to understand.  We have found that many errors students come across have nothing to do with Express, Vue, or any other library/framework.  Instead the errors come from mis-understanding one of these pure JS concepts:
* Assignment vs. Comparison
* Chainined Assignments
* [Value Swap](./value-swap)
* Variables are __untyped__
* [Reference vs. Value](./reference-vs-value)
* [Hoisting](./hoisting)
* [Dot vs Bracket Access](./dots-vs-brackets)

__Tutorials and the like:__
* [JavaScript.info](http://javascript.info/) chapters:
  * 2.1 -> 2.9
  * 4.1 -> 4.2
  * 5.1 -> 5.5
* Practical JavaScript:
  * [Basic Syntax](https://shawnr.gitbooks.io/practical-introduction-to-javascript/content/basic-syntax/)
  * [Data Types and Structures](https://shawnr.gitbooks.io/practical-introduction-to-javascript/content/data-types/)
* FreeCodeCamp on Variables:
  * FCC is a great place to start coding.  It has good exercises, good learning environment, and strong community.
  * [intro & basics](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript)
  * es6: [let vs var 1](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/es6/explore-differences-between-the-var-and-let-keywords), [let vs var 2](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/es6/compare-scopes-of-the-var-and-let-keywords), [const](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/es6/declare-a-read-only-variable-with-the-const-keyword)
  * [data structures](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-data-structures)
* You Don't Know JS:
  * [Types](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20%26%20grammar/ch1.md)
  * [Values](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20%26%20grammar/ch2.md)
  * [Type Coersion](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20%26%20grammar/ch4.md)

__Visualization Tools:__
* [PythonTutor for JavaScript](https://github.com/elewa-academy/js-tool-kit/blob/master/learning-environments.md#pythontutor):
  * For building your Notional Machine: visualizes how the JavaScript engine steps through code, deals with variables, and handles control flow. 
  * Copy your code into the text area and click "visualize execution".  Step through line by line with the "forward" button.  
* [Parsonizer](https://github.com/elewa-academy/js-tool-kit/blob/master/learning-environments.md#parsonizer):
  * Randomizes the lines in your code, you have to put them back in order (white space counts!).  This will help you learn syntactic structures & develop your logical problem solving skills by studying quality examples.
  * Copy paste your code into the text box and click the magic button.  Click "get feedback" to grade your answer.



__Tricky Bits:__
* Creation vs Execution phases:
  * _Creation phase_ is what happens before the first line is executed.  Mostly just hoisting. You can see what happened in the creation phase, it's what PythonTutor displays before you click the __forward__ button for the first time.
  * _Execution phase_ is everything that happens after the creation phase.
* JavaScript Types:
  * [Primitives vs. Objects](https://codeburst.io/javascript-data-types-explained-347555cd2d4d)
  * [List of them](https://www.w3schools.com/js/js_datatypes.asp)
  * [Type Coersion](https://javascriptweblog.wordpress.com/2010/09/27/the-secret-life-of-javascript-primitives/)
* Expressions vs. Operators:
  * (This is a tricky concept, it will make more sense after __Scope & Flow Control__)
  * Over Views:[dev.to](https://dev.to/promhize/javascript-in-depth-all-you-need-to-know-about-expressions-statements-and-expression-statements-5k2), [flaviocopes](https://flaviocopes.com/javascript-expressions/), [lib.ru](http://lib.ru/%3E%3C/JAVA/javascr/expr.html)
  * In Depth: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators), [2ality](http://2ality.com/2012/09/expressions-vs-statements.html)
  * Assignment vs Comparison: [Overview (study with PyTut)](https://www.quirksmode.org/blog/archives/2008/01/using_the_assig.html#link1), [This isn't just a JS thing](http://wiki.c2.com/?AssignmentVsEqualityOperator)
* Assign by reference vs. value: 
  * [Gist to study](https://gist.github.com/colevandersWands/9f50787fdddfb195d181da94c25536d8)
  * [article 1](https://codeburst.io/explaining-value-vs-reference-in-javascript-647a975e12a0)
  * [article 2](https://medium.com/@naveenkarippai/learning-how-references-work-in-javascript-a066a4e15600)
* Hoisting: 
  * [Article to study with PyTut](https://john-dugan.com/hoisting-in-javascript/)
  * [JS is Compiled](https://medium.com/@nickbalestra/javascripts-lexical-scope-hoisting-and-closures-without-mystery-c2324681d4be)
  * [Creation phase](http://tramaine.me/blog/javascript-variables-and-functions-are-hoisted-prior-to-execution)
  * [Step-through example](./hoisting-example-step-through.md)
  * [Great gist](https://gist.github.com/rishabhgupta/06921ed0fb442071018fc3d643a3f913)
* Scope:
  * [gist to study](https://gist.github.com/colevandersWands/557c6f7f770eaecfcb6216c893e69166)
  * [w3schools](https://www.w3schools.com/js/js_scope.asp)
  * [Let vs var](https://codeburst.io/difference-between-let-and-var-in-javascript-537410b2d707)
  * [Issues with 'var'](https://www.youtube.com/watch?v=7tGmS2SPxBo)
  * [in great detail](http://exploringjs.com/es6/ch_variables.html)
* [Incrementing & Decrementing](https://codeburst.io/javascript-increment-and-decrement-8c223858d5ed)
* Memory Management & Garbage Collection:
  * [Over-view](https://codeburst.io/javascript-memory-management-and-garbage-collection-in-javascript-ebe7a97d7143)
  * [In-depth](https://javascript.info/garbage-collection)


[TOP](#variables-&-types)

___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>

