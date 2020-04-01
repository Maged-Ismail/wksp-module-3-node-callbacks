# Questions

**With a partner**, answer these questions as completely as possible. Feel free to look at past lecture notes, the web, anything. 

Take the time to explain it to each other. 

The power of this exercise is in the act of _formulating_ and _explaining_ the concepts to someone else (your teammate).

## One

Run the app. Write out the steps, the _pseudo code_, required to create this app. It doesn't have to be totally accurate, or in the right order.

Only move on to the next question when you have enough detail that you would be able to start coding it yourself.

```
// create an html file
// add a header
// add a form
// store the value of the input in a variable
// add the variable to a list item in a div
// 

```

## Two - `server.js`

Take a look at the `server.js` file.

We have a new module in there, `body-parser` that is required on line `4`. What is it for? What is its use-case? What other lines are related to this module?

_The NPM site might be a good place to start. Feel free to provide links as relevant._

```
// It is used to identify the source of the request
// it distinguishes the difference between a browser request (html) and a server request(json)
// line 18 in server.js & lines 17 to 30 in handlers.js

```

## Three - `server.js`

Look at lines `23` and `24`. Explain the methods used. How are they different? What are the usecases for each?

```
// line 23 calls handleHomePage function when there is a request
''line 24 calls handleFormData function when the submit button is pressed

```

## Four - `server.js`

Line `6`. That's new. What do you think it's for?

```
// to import the function from the handlers.js file

```

## Five - `handlers.js`

Explain line `1`. Where, why and how is `items` being used?

```
// items is being declared as an empty array, everytime function handleFormData is called, the input is pushed and stored into ''items''. 

```

## Six - `handlers.js`

Why is there `redirect` on line `11`;

```
// everytime an item is added, the page reloads with the new data

``` 

## Seven - `handlers.js`

The `handle404` function is a more complex than we've seen thus far, what is the extra functionality for?

```
// If the request comes from a browser, than page fourOhFour is rendered;
//if the request is from another server (JSON), an error message is send
// 'Not Found' is sent in any other cases

```

## Eight - `ejs`

Take a look at `homepage.ejs` and `todoInput.ejs`. What is happening in there? Explain line-by-line...

```
// 1 - renders the partial file 'header';
// 2 - creates a new div in the body (for styling)
// 3 - render the partial file ' todoInput' which is the form
// 4 - Closes that div
// 5 - creates a new div
// 6 - creates an unordered list
// 7, 8 & 9 - Creates a loop to take each element in 'items' and makes a new item list for it
// 10 - Closes the list
// 11 - Closes the div
// 12 - renders the partial file 'footer'

```

## Nine - `styles.scss`

What are lines `2` to `7` for this file? Where are these values being used? Take a look at `_homepage.scss` as well? What do you notice?

```
// These are variable declaration' they are used in the styling files to avoid repetition and is easier to change

```

## Ten - `_homepage.scss`

Line `16`. See if by searching the Sass documentation, you can determine what _exactly_ is going on here. That `#{}` notation very specific to this use-case. Why?

```
// it's used for variable interpolation just like the backtics in javascript

```







