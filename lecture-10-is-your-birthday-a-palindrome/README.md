# Mark 13: Is your birthday a palindrome
### Array methods
- ### split()
    - split method splits a string into an array of substrings
    - returns a new array 
    - separator can be specified, the default is comma
    - Syntax:
      <pre>string.split(separator)</pre>
    - Example:
        <pre>var text = "NeogCamp admissions 2022";
        console.log(text.split(‘ ‘));
        Output:
        ['NeogCamp', 'admissions', '2022']</pre>

- ### reverse()
    - reverse method reverses the elements of an array
    - overwrites the original array
    - Syntax:
      <pre>array.reverse()</pre> 
    - Example:
        <pre>var cart = [“milk”,”eggs”,”bread”];
        console.log(cart.reverse());
        Output:
        [“bread”,”eggs”,”milk”]</pre>

- ### join()
    - join method joins all the array elements into a string.
    - returns an array as a string
    - separator can be specified, the default is comma
    - Syntax:
        <pre>array.join(separator);</pre>
    - Example:
        <pre>var textArray = [“milk”,”eggs”,”bread”];
        console.log(textArray.join(“-”));
        Output:
        milk-eggs-bread</pre>

- ### slice()
    - slice method returns a new array with the selected elements in an array.
    - It accepts two parameters, start and end.
    - If start parameter is not specified, it takes the default value as 0
    - If the end parameter is not specified, it starts selecting from the start index and goes up to the end of the array.
    - Use negative numbers to select from the end of the array
    - Starts selecting from the start index and goes up to the end index which is not inclusive.
    - Syntax:
        <pre>array.slice(start,end);</pre>
    - Example:
        <pre>var textArray = ['NeogCamp', 'admissions', '2022','interviews'];
        console.log(textArray.slice(0,3));
        Output:
        ['NeogCamp', 'admissions', '2022']</pre>

- ### push()
    - push method adds new items to the end of the array
    - any number of items can be pushed at once
    - returns a number that is the length of the array
    - Syntax:
        <pre>array.push(item1,item2,....,itemX);</pre>
    - Example:
        <pre>var cart = [“milk”,”eggs”,”bread”];
        console.log(cart.push(“tea”,”coffee”));
        console.log(cart);
        Output:
        5
        [“milk”,”eggs”,”bread”,“tea”,”coffee”]</pre>

- <a href="https://www.w3schools.com/js/js_array_methods.asp">Read more about array methods</a>

### `return` in JavaScript
- `return` statement stops the execution of the function and returns a value from that function
- If the value is not specified, it returns undefined.
- Syntax:
    <pre>return value;</pre>
