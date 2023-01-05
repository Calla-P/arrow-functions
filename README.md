# ES6 Arrow Functions

This assignment is designed to introduce you to some features in ECMAScript 2015{:target="_blank"}, otherwise known as ES6. From this point on, you are expected to use these features.

## Overview: Arrow Functions

MDN docs{:target="_blank"}
caniuse.com{:target="_blank"}
By now you should be comfortable writing function expressions{:target="_blank"} and function declarations{:target="_blank"}. Arrow functions are a shorter, more concise way to write a JavaScript function. The syntax might seem strange at first, so try to use arrow functions wherever you can and they will become second nature in no time.

There are a few caveats with arrow functions, though. Most importantly, the this context is not reset within an arrow function. The value of this is therefore the same as the this of the enclosing scope (the surrounding non-arrow function). If there isn't a non-arrow function scope surrounding, the this context will be, in the browser, the global window object.

Why does this happen? It happens because arrow functions retain the this value of the enclosing functional scope. Therefore, you will want to avoid using an arrow function in a constructor (where we need the contextual this to be the object we are building) or any method that needs to use this to behave properly.

## Assignment Tasks

1. Create a new repo in your GitHub account called arrow-functions. Clone the empty repo to your dev environment.
2. Navigate to the prework folder in the root directory of the class repository. Then navigate into the arrow-functions folder.
3. Copy the contents of the folder named starter-code into your newly-created repo. Make an initial commit with the unchanged starter code.
4. Proceed to work on a well-named branch. As you work, remember to add, commit, and push regularly.
5. The app.js file contains examples of function expressions, as you are accustomed to seeing. Work through steps 1-9, reading the notes and reviewing the refactored samples.
6. For each of these steps, uncomment the console.log line. Open the index.html file in the browser and verify the correct output in the developer console.
7. To complete step 10, refactor the function expressions one at a time. Uncomment the console.log line and use it to check that the output is the same after you have completed the refactoring process.
8. To complete step 11, uncomment the two console.log lines and observe the output in the developer console in the browser. Answer the corresponding questions.

## Additional resources

"JavaScript Arrow Functions" by Wes Bos{:target="_blank"}

## Submission Instructions

1. When finished, make a PR from your branch to main, and merge it.
2. Submit a link to your PR. You can link to a pull request even if the pull request is already merged or closed.
3. Add a comment in your Canvas assignment which includes the following:

- A question within the context of today's lab assignment
- An observation about the lab assignment, or related 'Ah-hah!' moment
- How long you spent working on this assignment