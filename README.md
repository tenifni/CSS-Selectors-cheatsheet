# CSS Selectors cheat sheet
notes from http://flukeout.github.io.




##Descendant Selector 
Select an element inside another element.

``` 
A  B -- Selects all B inside of A.
``` 

``` CSS
#fancy  span -- Selects any <span> descendant of any element with id="fancy"
```
</ul>

##Combine Class Selector
We can combine the class selector with other selectors.
```
A.className
```
``` CSS
ul.important -- selects all <ul> elements that have class="important"
```

##Comma Combinator 
Combine selctors with commas.
```
A, B
```
``` CSS
p, .fun, div -- selects all <p> elements, elements with class="fun" and <div> elements
```

##Universal Selector 
Combine class selector with other selectors.

```
*
```
``` CSS
p * -- Selects every element inside all <p> elements.
```

##Adjacent Sibling Selector 
Selector an element that directly follows another element.
```
A + B -- Selects all B elements that directly follow A
```
```
p + .intro -- Selects every element with class="intro" that directly follows a <p>
```


##General Sibling Selector 
Select elements that follows another element.
```
A ~ B --  Selects all B elements that follow a A
```

##Child Selector 
Select direct child of an element.
```
A > B --  Selects all B that are a direct child of A
```

##First Child Pseudo-selector 
Select the first child element inside of another element.
```
 :first-child
```

```CSS
div p:first-child -- Selects all first child <p> elements that are in a <div>
```


##Only Child Pseudo-selector 
Select an element that is the only element inside of another element.
```
 :only-child
```

```CSS
ul li:only-child -- Selects the only <li> element in a <ul>.
```


##Last Child Pseudo-selector 
Select the last element inside of another element.  
Use this selector to select an element that is the last child element inside of another element.  
**_Pro Tip_:** In cases where there is only one element, that element counts as the first-child, only-child and last-child!
```
:last-child
```
```CSS
ul li:last-child -- Selects the last <li> elements inside any <ul> 
```


##Nth Child Pseudo-selector
Select an element by its order in another element.
```CSS
:nth-child(#)
```
```CSS
div p:nth-child(2) -- Selects the 2nd <p> in any <div>
```


##Nth Last Child Selector
Select an element by its order in another element, counting from the back.

```CSS
:nth-last-child(#)
```


##First of Type Selector
Select the first element of a specific type.
```
:first-of-type
```
```CSS
span:first-of-type -- Selects the first <span> in any element.
```

##Nth of Type
Selects a specific element based on its type and order in another element - or even or odd instances of that element.
```
:nth-of-type(#)
```
```CSS
.example:nth-of-type(odd) -- Selects all odd instances of a the "example" class.
```


##Nth of Type Selector with Formula
Select every nth element, starting the count at a specific instance of that element.
```
:nth-of-type(An+B)
```
```CSS
span:nth-of-type(6n+2) -- Selects every 6th instance of a span, starting from (and including) the second.
```

##Only of Type
Select elements that are the only ones of their type within of their parent element.
```
:only-of-type
```
```CSS
p span:only-of-type -- Selects the <span> within any <p> if it is the only <span> in there.
```


##Last of Type
Select the last element of a specific type.

```
:last-of-type
```

```CSS
p span:last-of-type -- Selects the last <span> in every <p>
```

##Empty Selector
Select elements that don't have any children.
```
:empty
```
```CSS
div:empty -- Selects all empty <div> elements
```

##Negation Pseudo-class
select all elements that do not match the negation selector "A"
```
:not(A)
```
```CSS
:not(#fancy) -- Selects all elements that do not have id="fancy"

:not(.big, .medium) -- Selects all elements that do not have class="big" or class="medium"
```

