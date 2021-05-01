# Review, Research, and Discussion

1. Array.map

The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

Syntax :

![ARRAY](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/401/ARRAY.jpg?raw=true)

2. Array.reduce

The reduce() method executes a reducer function on each element of the array, resulting in a single output value.

The reducer function takes four arguments:

A- Accumulator
B- Current Value
C- Current Index
D- Source Array

Syntax :

![reduce](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/401/reduce.jpg?raw=true)

3. superagent

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs.

A- Install

npm install superagent

B- Usage

const superagent = require('superagent');

C- callback

superagent
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' }) // sends a JSON post body
  .set('X-API-Key', 'foobar')
  .set('accept', 'json')
  .end((err, res) => {
    // Calling the end function will send the request
  });

promise with then/catch

superagent.post('/api/pet').then(console.log).catch(console.error);

4. .then

The then() method returns a Promise. It takes up to two arguments: callback functions for the success and failure cases of the Promise.

Syntax :

![then](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/401/then.jpg?raw=true)

5. async

A Promise is an object representing the eventual completion or failure of an asynchronous operation.

A promise is a returned object to which you attach callbacks, instead of passing callbacks into a function.

Syntax :

function successCallback(result) {
  console.log("Audio file ready at URL: " + result);
}

function failureCallback(error) {
  console.error("Error generating audio file: " + error);
}

createAudioFileAsync(audioSettings, successCallback, failureCallback);

6. Async/await

A- AWAIT

let value = await promise;

B- ASYNC

async function f() {
  return 1;
}


An async function is a function declared with the async keyword, and the await keyword is permitted within them. The async and await keywords enable asynchronous, promise-based behavior to be written in a cleaner style, avoiding the need to explicitly configure promise chains.

There’s a special syntax to work with promises in a more comfortable fashion, called “async/await”. It’s surprisingly easy to understand and use.

Syntax :

async function f() {
  return 1;
}

f().then(alert);