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
