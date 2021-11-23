# Mark 13: Is your birthday a palindrome
### Array methods in JavaScript
- ### [`split()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)
    - `split()` method splits a **string** into an array of substrings
    - returns a new array 
    - separator can be specified, the default is comma
    - Syntax:
      <pre>string.split(separator)</pre>
    - Example:
        <pre>  var text = "NeogCamp admissions 2022";
        console.log(text.split(‘ ‘));
        Output:
        ['NeogCamp', 'admissions', '2022']</pre>

- ### [`reverse()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)
    - `reverse()` method reverses the elements of an array
    - overwrites the original array
    - Syntax:
      <pre>array.reverse()</pre> 
    - Example:
        <pre>  var cart = [“milk”,”eggs”,”bread”];
        console.log(cart.reverse());
        Output:
        [“bread”,”eggs”,”milk”]</pre>

- ### [`join()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)
    - `join()` method joins all the array elements into a string.
    - returns an array as a string
    - separator can be specified, the default is comma
    - Syntax:
        <pre>array.join(separator);</pre>
    - Example:
        <pre>  var textArray = [“milk”,”eggs”,”bread”];
        console.log(textArray.join(“-”));
        Output:
        milk-eggs-bread</pre>

- ### [`slice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice)
    - `slice()` method returns a new array with the selected elements in an array.
    - It accepts two parameters, start and end.
     - Starts selecting from the start index and goes up to the end index which is not inclusive.
    - If start parameter is not specified, it takes the default value as 0
    - If the end parameter is not specified, it starts selecting from the start index and goes up to the end of the array.
    - Use negative numbers to select from the end of the array
    - Syntax:
        <pre>array.slice(start,end);</pre>
    - Example:
        <pre>  var textArray = ['NeogCamp', 'admissions', '2022','interviews'];
        console.log(textArray.slice(0,3));
        Output:
        ['NeogCamp', 'admissions', '2022']</pre>

- ### [`push()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push)
    - `push()` method adds new items to the end of the array
    - any number of items can be pushed at once
    - returns a number that is the length of the array
    - Syntax:
        <pre>array.push(item1,item2,....,itemX);</pre>
    - Example:
        <pre>  var cart = [“milk”,”eggs”,”bread”];
        console.log(cart.push(“tea”,”coffee”));
        console.log(cart);
        Output:
        5
        [“milk”,”eggs”,”bread”,“tea”,”coffee”]</pre>
- ### [`sort()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)
    - The `sort()` method sorts the elements of an array (lexicographically) in place and returns the sorted array.
    - Syntax
        <pre>arr.sort()</pre>
    - Example
        <pre>
        const array1 = [1, 30, 4, 21, 100000];
        array1.sort();
        console.log(array1);
        output:  [1, 100000, 21, 30, 4]<pre>
- ### [`indexOf()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf)
    - The `indexOf()` method returns the first index at which a given element can be found in the array, or -1 if it is not present.
    - Syntax
        <pre>indexOf(searchElement)<br/>indexOf(searchElement, fromIndex)</pre>
    - Parameters
        - searchElement<br/>
            The element to be located.
        - fromIndex (Optional)<br>
            The index to start the search at.
    - Example 
        <pre>const beasts = ['ant', 'bison', 'camel','duck', 'bison'];

        console.log(beasts.indexOf('bison'));
        // expected output: 1

        // start from index 2
         console.log(beasts.indexOf('bison', 2));
        // expected output: 4</pre>

- <a href="https://www.w3schools.com/js/js_array_methods.asp">Read more about array methods</a>

### `return` in JavaScript
- `return` statement stops the execution of the function and returns a value from that function
- If the value is not specified, it returns undefined.
- Syntax:
    <pre>return value;</pre>


### Iterating within an array
- ### [`forEach()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
    - `forEach()` executes the callback function once for each array element
    - Syntax :
        <pre>array.forEach(function(currentValue, index, arr), thisValue)</pre>
    - Parameters 
        - callbackFn<br/>
        Function to execute on each element.
        It accepts between one and three arguments:
        - element<br />
         The current element being processed in the array.

        - index (Optional) <br/> 
            The index of element in the array.

        - array (Optional) <br/>
            The array forEach() was called upon.

        - thisArg (Optional) <br/>
            Value to use as this when executing callbackFn.

    - Example
        <pre>
        let sum = 0;
        const numbers = [65, 44, 12, 4];
        numbers.forEach(myFunction);

        function myFunction(item) {
        sum += item;
        }
        Output: 125</pre>

- ### [`every()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/every)
    - It returns a boolean - true if every element in this array satisfies the provided testing function. 
    - An important difference with `every()` is that the test function may not always be called for every element in the array. Once the testing function returns false for any element, no more array elements are iterated.
    - Syntax: 
        <pre>arr.every(callback(element[, index[, array]])[, thisArg])</pre>
    - Parameters
        - callbackFn - A function to test for each element, taking three arguments:

        - element<br/>
         The current element being processed in the array.

        - index (Optional)<br/>
        The index of the current element being processed in the array.

        - array (Optional)<br/>
        The array on which  every() was called upon.

        - thisArg (Optional)<br/>
        A value to use as this when executing callbackFn.
    - Example
        <pre>const isBelowThreshold = (currentValue) => currentValue < 40;

        const array1 = [1, 30, 39, 29, 10, 13];

        console.log(array1.every(isBelowThreshold));
        Output: true</pre>
 
- ### [`map()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
    - The `map()` method creates a new array populated with the results of calling a provided function on every element in the calling array.
    - returns a new Array of objects created by taking some action on the original item.
    - Parameters 
        - callbackFn - Function that is called for every element of arr. Each time callbackFn executes, the returned value is added to newArray.
        - The callbackFn function accepts the following arguments:

        - element<br/>
        The current element being processed in the array.

        - index (Optional)<br/>
        The index of the current element being processed in the array.

        - array (Optional)<br/>
        The array map was called upon.

        - thisArg (Optional)<br/>
        Value to use as this when executing callbackFn.
    - Example 	
        <pre>const array1 = [1, 4, 9, 16];

        // pass a function to map
        const map1 = array1.map(x => x * 2);

        console.log(map1);
        Output: Array [2, 8, 18, 32]</pre>
- ### [`filter()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)
    - The `filter()` method creates a new array with all elements that pass the test implemented by the provided function.
    - Parameters :
        - callbackFn - Function that is called for every element of arr. Each time callbackFn executes, the returned value is added to newArray.
        - The callbackFn function accepts the following arguments:

        - element<br/>
            The current element being processed in the array.

        - index (Optional)<br/>
            The index of the current element being processed in the array.

        - array (Optional)<br/>
            The array map was called upon.

        - thisArg (Optional)<br/>
            Value to use as this when executing callbackFn.
    - Example 
        <pre>const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

        const result = words.filter(word => word.length > 6);

        console.log(result);
        Output: Array ["exuberant", "destruction", "present"]</pre>

- ### [`some()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/some)
    - The `some()` method tests whether at least one element in the array passes the test implemented by the provided function. 
    - It returns true if, in the array, it finds an element for which the provided function returns true; otherwise it returns false.
    - Parameters :
        - callbackFn - Function that is called for every element of arr. Each time callbackFn executes, the returned value is added to newArray.
        - The callbackFn function accepts the following arguments:

        - element<br/>
            The current element being processed in the array.

        - index (Optional)<br/>
            The index of the current element being processed in the array.

        - array (Optional)<br/>
            The array map was called upon.

        - thisArg (Optional)<br/>
            Value to use as this when executing callbackFn.

    - Example 
        <pre>const array = [1, 2, 3, 4, 5];

        // checks whether an element is even
        const even = (element) => element % 2 === 0;

        console.log(array.some(even));
        Output: true</pre>


### Iterating through an object 
### [`Object.keys()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)
- The `Object.keys()` method returns an array of a given object's own enumerable property names, iterated in the same order that a normal loop would.
- Syntax 
    <pre>Object.keys(obj)</pre>
- Example
    <pre>const object1 = {
    a: "apple",
    b: "banana",
    };

    console.log(Object.keys(object1));
    Output: [“a”,“b”]</pre>

### [`Object.values()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/values)
- The `Object.values()` method returns an array of a given object's own enumerable property values
- Syntax 
    <pre>Object.values(obj)</pre>
- Example
    <pre>const object1 = {
    a: "apple",
    b: "banana",
    };

    console.log(Object.values(object1));
    Output: ["apple", "banana"]</pre>
