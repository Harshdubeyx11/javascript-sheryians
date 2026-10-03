# JAVASCRIPT

## Keywords 
- special words in js which have some functionality

## variables 
- where we store values/data
- in JS we have 3: var , let , const (but we dont use var now)
- let: we use when we have to change value in future (example a score which keeps chaning)
- const - for fixed value(Example pi value)
- var: They are added in window in dev tools console
- var: they are function scoped only so if in a function we have if statemenet then inside it we have var assignend then we can use that var inside the whole function and not just under the if statement which is bad , and var has to be inside a function it wont work inside just a block without any function mentioned
- <img width="187" height="117" alt="image" src="https://github.com/user-attachments/assets/ec9791e4-2537-4398-ba88-5da2ca6b6fbb" /> (can use a=12 anywhere in function abcd)

- var: we can declare them again with same name wihout any error
- <img width="143" height="50" alt="image" src="https://github.com/user-attachments/assets/c0c2e531-24f2-430a-b1f9-101d85cd3bae" /> (which is a problem so always use "let")

###const
- we cant reassign a value but we can update the value
- <img width="272" height="50" alt="image" src="https://github.com/user-attachments/assets/d2567605-e902-4679-8461-1c9d75d6d14b" />


## Scope

### global scope: can be used anywhere

### block scope 
- variables which can be used in that block only (meaning inside that brackets only) : like "let" variable

### function scoped 
- variables which can be accessed in the full function like "var"

## Redeclaration of variables:
- <img width="128" height="51" alt="image" src="https://github.com/user-attachments/assets/31ae44a1-e503-416d-a5f2-8be90c5102eb" />

## Temporal dead zone
- It is the area or (no of lines of a code) where js knows that "x" variable exists somewhere in code but since we are getting value of that variable before declaring it so it says it cant give you the value of that variable. 
- <img width="154" height="90" alt="image" src="https://github.com/user-attachments/assets/988f5e2c-81dd-4df6-a565-6674d950bca3" /> (here "a" is being printed in the first line before even declaring variable "a" in the 3rd line)
- so temporal dead zone here is from line 1 till 2
- Temporal dead zone: happens in "let" and "const" but not in "var"


## Hoisting
- When we make a variable in JS -It breaks into 2 parts: variable part and initialization part
- so the variable goes to the top of the code and then initialized value remains at the bottom - this is called hoisting
- <img width="156" height="80" alt="image" src="https://github.com/user-attachments/assets/b0fecf36-04ef-4512-b064-e54b759c9c57" />(that's why here also it knows a exists but cant print its value as it is at the bottom)


## Data-types
- 2 types: primitives and references
- primitives: datatypes which dont have any brackets (string , number , bool , null , undefi ed, symbol, bigINT)
- references: have brackets - eg arrays[] , objects {} , tuples ()
- null: means you delebrately did not have any value , as till now we dont know what that value is.
- undefined: you made a variable and did not initialise it with a value so the value it gets is undefined

## how to add +1/+2 etc to the maximum value an integer can hold
- max value an integer can hold = Number.MAX_SAFE_INTERGER
- so you have to put "n" at its last
- let a = 9007199254740991n <----
- then you can do a = a +2n etc (to add +2)

## References are array[] , objects{} , tuples()
- <img width="173" height="82" alt="image" src="https://github.com/user-attachments/assets/f9dab06f-13f6-4089-9aff-b2d6e6063166" /> (here b is a reference to a for any change in b will change 'a')


## Dynamic Typing
- there is no static typing in JS
- JS has dynamic data types (meaning if a=12 it can later become a=true so integer to bool)

## Type coercion (== vs ===)
- In JS we can add two different types of data types
- <img width="95" height="53" alt="image" src="https://github.com/user-attachments/assets/010c209b-aa92-4426-afeb-7a5c74a0a6b0" /> (here 1 was also considered as string and concatenated with "5")
- why was 5 not considered integer and additon did not happen - because if any of the operands are string then JS thinks other is also string
- <img width="96" height="52" alt="image" src="https://github.com/user-attachments/assets/044c9aa8-2d08-4b49-85b9-b4755bcaf5f6" /> ('+' operator does 2 things add and concatenate but '-' operator only subtracts)

## Truthy and falsey values
- In js if true/false is not mentioned then automatically as per value it takes true or false values
- JS consideres all ( 0 , false , "" , null , undefined , NaN , document.all) as false values
- rest all are true

## What is true + false
- true = 1 and false = 0 so 1+0=1

## What is null+1
- null = 0 so null+1 = 0+1 = 1

## why NaN(not a number) is a number
- NaN is Js is a failed number operation
- so if you multiply ---> 2 * 'harsh" we get a value called NaN(not a number)
- since it was a number operation but it failed so its a NaN

## Difference between undefined and null
- <img width="340" height="88" alt="image" src="https://github.com/user-attachments/assets/4b77e159-4371-45da-9995-61e0d08929d1" />

## Arithematic operators
<img width="218" height="115" alt="image" src="https://github.com/user-attachments/assets/ac066fdc-85cb-4a90-824c-d600295b979d" />

## How is == different from ===
- 12 == '12' -----> true (does not check datatype
- 12 === '12' ----> false (checks datatype also)

## Problem in JS
- (typeof null) ---> gives 'object' ->wrong
- (typeof array) ---> gives 'object' ->wrong

## Control flow statements
- if else
- switch cases
- early return patterns
  
## Loops
- for loop , while loop , foreach loop , do-while , 
- <img width="96" height="94" alt="image" src="https://github.com/user-attachments/assets/b67c0cc1-948d-49e7-99c2-20e1b6be0b2a" /> (while loop syntax)
- <img width="174" height="120" alt="image" src="https://github.com/user-attachments/assets/a11b615c-8c8d-4f36-a694-bee4b93aa2e4" /> (do-while loop syntax)
- one interesting thing about do while loop is that it always atleast interates for once (atleast once) - even if the conditons are not met still


## Functions
### usecase
- we make functions so that a particular block of code only works when it is called and does not work if its not called
- secondly, we can reuse the functions

### how to write functions
- <img width="149" height="85" alt="image" src="https://github.com/user-attachments/assets/bc0f85cb-c84f-42ce-913e-787105c85c48" /> (directly creating function) -> this method is called function statement
- <img width="272" height="123" alt="image" src="https://github.com/user-attachments/assets/c78ef661-61bd-4495-bc91-f7f1e75e01aa" /> (initializing fucntion by a variable - here the function name is "fnc") -> this method is called function expression
- <img width="226" height="96" alt="image" src="https://github.com/user-attachments/assets/0ccf0976-ff70-4095-8b0d-e6b3d18b9e63" /> (called fat arrow function)

## Parameters and Arguments in Functions
- <img width="304" height="176" alt="image" src="https://github.com/user-attachments/assets/08552a74-6171-4b99-bbb2-5d15dc3a15c4" />
- so you can put "`${x}`" to then call functions by any value you want
- <img width="189" height="120" alt="image" src="https://github.com/user-attachments/assets/70d53c15-f270-4ca4-b1d8-71c8a745dffa" /> (here v1, v2 are parameters and 1,2 are arguments)

### default parameters
- <img width="239" height="100" alt="image" src="https://github.com/user-attachments/assets/d206b86e-c93d-4069-8e36-f015c18b8119" /> (if no values present then we can give default values in the parameters here we have given 0)

### Rest & Spread
- If in a function we have a lot of arguments so we will have to make that many parameters, but thats not possible with a lot of arguments say 1000 so to get rid of this problem we use REST(...) or Spread(...)
- if we put "..." in the function parameters then its ---> Rest
- if we put "..." in the arrays or objects then its ---> Spread 
- <img width="270" height="124" alt="image" src="https://github.com/user-attachments/assets/25e93bec-a2ea-42ed-b1fa-48882d7d2e64" />
- we can also do like 1,2,3 in variables and remaining in REST like:
- <img width="341" height="118" alt="image" src="https://github.com/user-attachments/assets/91686c6b-1dfb-42dc-9968-97e30b4598a4" />


## First class functions
- functions which we can treat as a "value" and can save it in variables

## Higher order functions
- A function which either has another funtion in its parameters or it returns another funtions inside it
- <img width="188" height="162" alt="image" src="https://github.com/user-attachments/assets/3013eaca-f08d-4152-b316-a63ade0de339" /> (top abcd is accepting a function in the parameter)
- <img width="226" height="159" alt="image" src="https://github.com/user-attachments/assets/9705af80-c5d5-41ca-ac41-d05aac89a0a8" /> (Returning a function inside a function)


## Pure vs Impure functions

- Pure function: A function which does not change any value outside of it
- <img width="253" height="118" alt="image" src="https://github.com/user-attachments/assets/5b5596c0-c71a-40c4-9450-514b4e710e2a" /> (no outside value is changing from this function)

- Impure function: A function which changes any value outside of it - means a function which has side affects outside of its scope
- <img width="161" height="77" alt="image" src="https://github.com/user-attachments/assets/401b6fdc-3033-4a14-a9ff-9bc345afec81" /> ("a" value is chaning)



## Closures (imp for interview)
- A function which returns another function inside it and the function which is getting returned(the inside one) - that function uses any variable of the parent function
- <img width="231" height="142" alt="image" src="https://github.com/user-attachments/assets/5d3cb565-7350-46e8-8768-67c4fb17f51b" />


## Lexical scoping (imp for interview)
- <img width="211" height="207" alt="image" src="https://github.com/user-attachments/assets/0b4fc77a-5a6b-4c57-95ab-b3ce02ffd099" />
- here a can be accessed in all 3 functions, b can be accessed in 2 fucntions and c can be accessed in 1 function
- so lexical scoping is the physical scope of the variables inside functions
  

## IIFE (immediately invoked function expressions)
- <img width="149" height="72" alt="image" src="https://github.com/user-attachments/assets/2b46b5f5-52b8-4f0e-92ba-e0f438dbe272" />
- This is an IIFE -> make a function and surround it with round brackets and just call it directly in the end
- Iske andar jo code likhdoge woh ussi time chal jayega


## Hoisting difference between declaration and expression

- 





