# Intro to Programming and Control Flow

## Objectives
*After this lesson, students will be able to:*
- Understand how to store and manipulate data using variables
- Understand what `for` and `if` statements are, and how we can utilize these control the program's "flow"
- Combine data and control flow statements to create **PROGRAMS** 🎉

# Variables, semicolons and curly braces; Oh my!

## How to use `var` to save our donuts
- A variable is a container you can store data in

```javascript
var numberOfDonuts = 13;
```
The keyword `var` signifies that we are about to create a new "container" or "variable" called `numberOfDonuts`.

The equals sign ( `=` ) is an `assignment operator`. It basically means, save the value `13` in our `numberOfDonuts` variable.

---

### The data types we'll be working with:
- String  - "The answer to Life, the Universe, and Everything JavaScript"
- Number  - 42
- boolean  - `true` / `false`

### The other data types
* Array  - [ "Harry", "Hermione", "Ron" ]
* Object  - { author: "J.K. Rowling" }

---

### Manipulating data
Operator | What it does | example
:--- | :---: | :---
| + | Addition | x = x + 1
| - | Subtraction | x = x - 1
| * | Multiplication | x = x * 1
| / | Division | x = x / 1
| ++ | Increment | x++
| -- | Decrement | x--


```javascript
var numDonuts = 1;

// Adding to my donuts
numberOfDonuts = numberOfDonuts + 1;

// Or alternatively:
numberOfDonuts++;
```

---

## Moving on... `if` ( we're ready === true )
* `if` statements only run IF the condition is true

```
// Psuedocode

If I am hungry  
    I will eat a donut
Else I won't eat
```


```javascript
var isHungry = true;

if(isHungry === true) {
    console.log("I have", numberOfDonuts, "donuts");
    numberOfDonuts--;
    console.log("I now have", numberOfDonuts, "donuts");
} else {
    console.log("I'm not hungry!");
}
```

---

## Looping structures - `for` and `while`
- `for` loops - loop through a block of code a specified number of times

```
// Psuedocode

For each finger on my hand
    I will count up by 1!
```

```javascript
console.log("Watch me count programmatically!");

for(var count = 1; count <= 5; count++) {
    console.log("Count is:", count);
}
```
- `while` loops - loop through a block of code while a specified condition is true


```
// Psuedocode

While I still have hot dogs on the table
    I will eat one hot dog!
```

```javascript
console.log("I'm going to eat all these hot dogs");
var numHotDogs = 10;

while(numHotDogs > 0) {
    numHotDogs--;
    console.log("After eating 1 hot dog, I have", numHotDogs, "hot dogs left to go!");
}

console.log("I ate all the hot dogs and won the contest!");
```

---

## Fun Functions! 
Code is read from top to bottom, left to right.
However, `function`s designate blocks of code that aren't executed until we invoke it.
```javascript
    var cookies = 10;
    cookies--;
    // We now have 9 cookies

    function eatACookie() {
        cookies--;
    }

    // We still have 9 cookies. eatACookie() will not run until we manually invoke it

    eatACookie();
    // After calling the function, we now have 8 cookies
```


# Putting our new skills into practice
## Let's build a thermometer app
This may sound scary, but we've got all the tools we need to do this

- Starter code can be found at 
https://codepen.io/username1124/pen/pqRGNW


# Recap
- Variables are containers for data
- We can assign values to those variables, or mutate the data inside however we like
- We learned how to run the same block of code multiple times with loops - `for` and `while`
- We learned to do some basic psuedocoding - basically laying out the structure of our logic with plain english
- We learned how to follow a program's flow - reading top to bottom, except where there's functions involved
