# Fun With Triangles 

## class and id?
for selection and to perform certain tasks in javaScript , we assign each element in Html with a class or an id.

> What is `class` ?
- A `class` is an attribute which is used to specify the class names for various Html elements. A class can be same for certain elements.
- Syntax 
```
<element class="class_name">
In CSS Stylesheet:
.class {
    // CSS Property
}
```

> What is `id`?
- An `id` is an attribute which is used to specify an unique html element. An id should be unique for every element. 
- Syntax 
```
<element id="id_name">

In CSS Stylesheet:
#id_name {
    // CSS Property
}
```

> Class Vs Id 
![Class Vs Id](classvsid.png)
## querySelectorAll n querySelector ka diff
all selects all 

index notation for selecting different elements of same class

## diff betn innerhtml n innertext
inner html new html elements
innertext puts text on already created tags

## why use form?
so that we can access it in js and things become easy
#all about forms
Methods 
formdata - is nothing but an API
> Syntax in js
> entry in formdata(key-value pair)
form ke andar button hoga to page gets refreshed

## input inside the label

## about radio button 
In radio group to toggle betwn the options we name them same.
radio buttons should have same name among the group. 
> name-
> value


## why addeventlistener and not onclick? 
do not put html under js and js under html n hence we use addeventListener as that is the best practice

## for of


* Syntax:
```
for (variable of iterable) {
  statement
}
```
> Eg:
![for of](forof.jpeg)


## Math in js
Math is a built-in object that has properties and methods for mathematical constants and functions. It’s not a function object.

Math works with the Number type. It doesn't work with BigInt(whole numbers larger than 2^53 - 1).


* Square root

 returns the square root of a number

> Syntax:
```
Math.sqrt()
```

> Example <br>
![example](matheg.jpeg)

# Know more:

[formData](https://developer.mozilla.org/en-US/docs/Web/API/FormData/FormData)

[Math in js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)

