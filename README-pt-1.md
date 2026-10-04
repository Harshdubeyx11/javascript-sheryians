# JAVASCRIPT PT-1

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
- if we put "..." in the function parameters then its ---> Rest (and the val parameter in the fucntion will act as an array of all the arguments/values)
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
- Hositing is when a variable is broken down into 2 parts its variable and its value and the variable goes up and value stays down so above the code knows that this variable exists but it cant give its value at that time
- mainly meaning the variable has been initialised and can be used before its even read at the bottom
- <img width="295" height="230" alt="image" src="https://github.com/user-attachments/assets/5f37ab18-3cba-41c5-924b-e39f91063cb3" /> (Hoisting in function declaration-----> WORKS)
- <img width="305" height="223" alt="image" src="https://github.com/user-attachments/assets/39401903-9fd8-4593-b49e-0b5fa6dfe73c" /> (Hoisting in function expression-----> DOES NOT WORK)
- so function declarations are Hoist whereas Function definition are not hoist


## QUESTION
- <img width="184" height="131" alt="image" src="https://github.com/user-attachments/assets/2b62f8bc-26ce-4157-be6a-99f27422d722" />
- this function will return undefined


## What does it mean when we say functions are first class citezens?

- means we can treat functions as just like values itself
- we can pass functions in functions , we can store it in variables 

## Objects
### Difference between arrays and objects 
- Arrays are for a lot of values
- we make objects when we want to know everything about one entity

- <img width="268" height="118" alt="image" src="https://github.com/user-attachments/assets/c9a54313-89c2-40db-a475-a7b7e2abdc23" /> (making an object)

### Accessing an object 
-  <img width="63" height="23" alt="image" src="https://github.com/user-attachments/assets/dec071e3-ac5b-4548-bcce-87e65bdad8f2" /> (if we use the method "obj." then whatever we write after the dot that exact thing will be serched in the object )
- <img width="82" height="23" alt="image" src="https://github.com/user-attachments/assets/5d187335-ab39-4f6a-ac69-48f825db0cad" /> (this is the square bracket method)
-  <img width="290" height="235" alt="image" src="https://github.com/user-attachments/assets/f2edd1c6-4183-4121-aaec-d4801488e692" />


### Deep object (object inside object)
- <img width="225" height="252" alt="image" src="https://github.com/user-attachments/assets/35e3443b-75c9-486a-867d-1a60063cc07a" />
- so if we want to access "lng" so we do:-- user.address.location.lng;
- <img width="356" height="29" alt="image" src="https://github.com/user-attachments/assets/04831460-81c2-4d7c-92cc-f7dd1aa516e1" /> (another way if you cant write such long line again and again to access then you can do it like this once then we can directly use lng or lat whatever)


### For loop in object
- <img width="279" height="208" alt="image" src="https://github.com/user-attachments/assets/302578e6-5866-49c1-927b-cc4d0715d41a" /> (to access all keys of object)
-  <img width="69" height="75" alt="image" src="https://github.com/user-attachments/assets/f2ad2c67-ebcf-48dc-9f41-19dd9ea35852" /> (output all keys printed)
-  <img width="285" height="204" alt="image" src="https://github.com/user-attachments/assets/9dd27f98-0ebd-4679-96a3-8cea85f6fe9c" /> (to access the values of all keys of object)
- <img width="120" height="75" alt="image" src="https://github.com/user-attachments/assets/d3f80b88-e499-4195-9cb8-4f584e452ae0" /> (outputs all values of keys in object)

### Object.keys() function ---> gives all the keys in array 
- <img width="280" height="169" alt="image" src="https://github.com/user-attachments/assets/10d222c1-462e-46d6-886e-cdbd144a2c84" />
- <img width="276" height="53" alt="image" src="https://github.com/user-attachments/assets/ed6a7061-bc5f-44bc-a20e-e3809ab7aac5" />

### Object.entries() function ---> gives all the (key,value) in array form
- <img width="192" height="24" alt="image" src="https://github.com/user-attachments/assets/d436f297-840e-4385-b979-049920a0f75e" />
<img width="217" height="55" alt="image" src="https://github.com/user-attachments/assets/79da81df-3b40-45b3-8c31-5df26d6d2a7f" />


### Spread operator in object
- can be used to copy an object into another object
- <img width="297" height="158" alt="image" src="https://github.com/user-attachments/assets/b1fd4bd7-364b-4ce1-85bb-b2dfd38c3efe" />
- <img width="374" height="44" alt="image" src="https://github.com/user-attachments/assets/0ff19a66-cd95-4b1a-b64d-3c949d1b949a" />

### If we make a nested object and then we declare another object2 and use spread operator or any operator to ocopy obj1 to obj2 and then change anything in the obj2 in the nested then in obj1 also it will be changed 

- <img width="323" height="249" alt="image" src="https://github.com/user-attachments/assets/2ee961ab-9c76-4c4b-942d-e0938feb94e1" />
- this is called deep-clone

### Another way to copy obj1 to obj2
- <img width="463" height="235" alt="image" src="https://github.com/user-attachments/assets/5e725607-d6cd-4358-bd70-829b438034ba" /> (first we convert to string by stringify then we parse it to its original form)
- if we now change anything in the nested place in obj2 then that wont create a deep copy and wont affect obj1
- So whenever you see a nested object and you want to copy it to another object use stringify and parse method and not spread operator method


### optional chaining 
- <img width="290" height="185" alt="image" src="https://github.com/user-attachments/assets/8588deb7-337b-4716-8bad-54da9dae22ca" />
- suppose we have this object and then later in the code very later, you change the address to salary
- so before you were calling like: obj.address.salary but it wont work because address changed to salary so you will get error
- so you can put like obj.address?.salary? question mark so we dont get error we get undefined


## One problem
- <img width="528" height="125" alt="image" src="https://github.com/user-attachments/assets/60f59ed5-6e32-4af3-8275-3be90ce30ecf" /> (correct method)
- <img width="531" height="109" alt="image" src="https://github.com/user-attachments/assets/1b85eee1-6684-45d4-b20c-820acc14bd71" /> (first-name dash is not allowed)












