https://youtu.be/x2RNw4M6cME by colt steele 


Primitive types in java script

    1. Number = 1,223, 4,121412
    2. String =  venkatesh
    3. Boolean = true, false
    4. Null = 0;
    5. Undefined = undefined

Numbers in JSON

    1. Positive Number
    2. negative Numbers
    3. Whole Numbers(integers)
    4. Decimal Numbers

simple operations

    1. Addition (+)
    2. Subraction (-)
    3. Multiplication (*)
    4. Division (/)
    5. Modulo (%)
    6. Exponentation (**)

NaN (not a number)

    NaN is a numeric value that represents something that is not a number
    >.0/0 = NaN
    >'f'/4 = NaN
    >1 + NaN = NaN

Variables

    Variable are like labled jars for a value in javascript
    syntax
    >let age = 55;

Const

    const values cannot be changed
    >const dogAge= 8;
    >dogAge +=8; error

var

var was the only way of declaring variables before "let" & "const"

Booleans

    >let isLoggedIn = true;  always lower case
    >const iHero = false;   always lower case

Variables can change type(Dynamic)

    >let isLoggedIn = 1;
    >console.log(isLoggedIn);
    ans = 1;

Strings

    comes with either with single quotes or double quotes
    >const firstName = "thomas";
    >let phrase = " I am a dummy";
    they are indexed (positioned and starts with '0'); accesed with []

String methods

    strings come with a set of build-in methods, which are actions that can be performed on or with that particular string

    1. Searching within a string
    2. replacing parts of a string
    3. Changing case (upper/lowercase)


    >msg.toUpperCase() & msg.toLowerCase() -> changes all the characters to uppercase and lowercase respectively

    msg.trim() -> cleans up unwanted spaces at the ends

msg.method(arg)

 arguments are data passed to the methods
    >let tvShow ="catdog";
    >tvShow.indexOf('cat');   // 0
    >tvShow.indexOf('dog');   // 3
    >tvShow.indexOf('z');    // not found

index 

    hello"[2]; // l

slice

    >"abcdef".slice(4)  //ef
    >"abcdef".slice(1,4) // bcede

replace

    >msg.replace('item1','replaced');

www.developer.mozilla.org // for reference

String template literals

template literals are strings that allow embedded expressions, which will be evaluated and then turned into a resulting string.
 
 `I counted ${3+5} sheep`;  // "I counted 7 sheep"
 back tick is used (``) not single quotes

null

    intentional abscence of a value which must be assigned

undefined

    variables that do not have a assigned value are undefined is a state

Boolean Logic result is always boolean 

    1. >     greater than
    2. <     less than
    3. >=    greater than or equal to
    4. <=    less than or equal to

    1. ==    equality  checks for equality of value, but not the equality of type  (better not use it)
    2. !=    not equal checks for equality of value, but not the type
    3. ===   strict equality check for equality of value and type (recommended)
    4. !==   strict non-equality (recommended)

console.log - is a method itself

Conditionals (Making decisions with code)

if statement

    let rating =3;
    if (rating ===3){
    console.log("nice");
    }

if else statement

    let score = 92;
    if (score > 90) {
        console.log("you got A grade")
    } else {
        console.log("you did not get an A")
    }


Math.random()  generates a random decimal number between 1 and 0

    if(expression){}
    else if(expression){}
    else if(expression){}
    else(){ }

nested Conditionals

    if(expression){
        if(expression){}
        else{}
    }
    else{}


Logic Operators (output is a boolean)

    1. && - AND  (both of the expression should be true inorder the output to be true)
    2. || - OR   (Either one of the expresssion should be true for the output to be true)
    3. !  - NOT  (returns true when false is received) - negation Operators

Arrays (collection of elements) - in JS elements need not to be of same type
Arraus are indexed like strings as [0,1,2,3,4,.....,n-1]

    let nums = [ 3, 31, 545, 'hello'];
    num[2][1] returns 5 // not a two dimensional array

Array methods

    1. Push - add to end
    2. Pop - remove from end and can be saved in a particular variable // video time 1:25:00
    3. shift - remove from the beginning
    4. unshift - add to the beginning

    concat - merge Arrays
    includes - looks for a value
    indexOf - just like str.indexOf
    join - creates a string from array
    reverse - reverses an array
    slice - copy a portion of an array
    splice - remove/replace elements
    sort - sorts an array

//const & Arrays








 






    




