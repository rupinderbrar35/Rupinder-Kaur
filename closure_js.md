A closure is an inner function that has access to the outer function's variables-Scope chain.
The closure has three scope chains:
1.It has access to its own scope(variable defined in its enclosing brackets).
2.It has access to the outer function'ss variables.
3.It has access to global variables.

The inner function has access not only to the outer function's variable's ,but alsa to the outer function's parameters. 

For Example:

var addTo = function(passed)

{
    
    var add = function(inner)
    
    {
        
        return passed + inner;
        
    }
    
    return add
    
}

console.log(addTo)



Here, inner function uses the variable'passed' which is defined in the outer function.


Closures are functions tha refers to independent variables (locally defined varibles, but defined in enclosing brackets).
In other words, these these functions don't forget the environment in which they are created.





References:


http://javascriptissexy.com/understand-javascript-closures-with-ease/

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures

https://www.youtube.com/watch?v=71AtaJpJHw0

http://www.w3schools.com/js/js_function_closures.asp
