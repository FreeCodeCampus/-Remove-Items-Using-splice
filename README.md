# Splice

## Basic Data Structures: Remove Items Using splice()

Ok, so we've learned how to remove elements from<br/>
the beginning and end of arrays using shift() and pop(),<br/> 
but what if we want to remove an element from somewhere in the<br/>
middle? Or remove more than one element at once?<br/>

Well, that's where splice() comes in. splice()<br/>
allows us to do just that: remove any number of<br/>
consecutive elements from anywhere in an array.<br/>

splice() can take up to 3 parameters, but for now,<br/>
we'll focus on just the first 2. The first two parameters of splice()<br/>
are integers which represent indexes, or positions, of the<br/>
array that splice() is being called upon. And remember,<br/>
arrays are zero-indexed, so to indicate the first element of<br/>
an array, we would use 0. splice()'s first parameter <br/>
represents the index on the array from which to begin removing<br/>
elements, while the second parameter indicates the number of elements to delete. For example:<br/>

let array = ['today', 'was', 'not', 'so', 'great'];<br/>

array.splice(2, 2);<br/>
// remove 2 elements beginning with the 3rd element<br/>
// array now equals ['today', 'was', 'great']<br/>
splice() not only modifies the array it's being called on, but it also returns a new array containing the value of the removed elements:<br/>

let array = ['I', 'am', 'feeling', 'really', 'happy'];<br/>

let newArray = array.splice(3, 2);
// newArray equals ['really', 'happy']

We've defined a function, sumOfTen, which takes an array as an argument and returns the sum <br/>
of that array's elements. Modify the function, using splice(), so that it returns a value of 10.

### To run this app
clone it :
```
git remote add origin git@github.com:FreeCodeCampus/Splice.git
```

and run a command in your terminal
```
node index.js
```
