# 1. CSS Selectors cheat sheet
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
Combine the class selector with other selectors.
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
:nth-child(X)
```
```CSS
div p:nth-child(2) -- Selects the 2nd <p> in any <div>
```


##Nth Last Child Selector
Select an element by its order in another element, counting from the back.

```CSS
:nth-last-child(X)
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
:nth-of-type(X)
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

##Empty 
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

# 2. Common CSS-JS properties Reference
from https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Properties_Reference.


<table>
 <thead>
  <tr>
   <th scope="col"><strong>CSS</strong></th>
   <th scope="col"><strong>JavaScript</strong></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>background</td>
   <td>background</td>
  </tr>
  <tr>
   <td>background-attachment</td>
   <td>backgroundAttachment</td>
  </tr>
  <tr>
   <td>background-color</td>
   <td>backgroundColor</td>
  </tr>
  <tr>
   <td>background-image</td>
   <td>backgroundImage</td>
  </tr>
  <tr>
   <td>background-position</td>
   <td>backgroundPosition</td>
  </tr>
  <tr>
   <td>background-repeat</td>
   <td>backgroundRepeat</td>
  </tr>
  <tr>
   <td>border</td>
   <td>border</td>
  </tr>
  <tr>
   <td>border-bottom</td>
   <td>borderBottom</td>
  </tr>
  <tr>
   <td>border-bottom-color</td>
   <td>borderBottomColor</td>
  </tr>
  <tr>
   <td>border-bottom-style</td>
   <td>borderBottomStyle</td>
  </tr>
  <tr>
   <td>border-bottom-width</td>
   <td>borderBottomWidth</td>
  </tr>
  <tr>
   <td>border-color</td>
   <td>borderColor</td>
  </tr>
  <tr>
   <td>border-left</td>
   <td>borderLeft</td>
  </tr>
  <tr>
   <td>border-left-color</td>
   <td>borderLeftColor</td>
  </tr>
  <tr>
   <td>border-left-style</td>
   <td>borderLeftStyle</td>
  </tr>
  <tr>
   <td>border-left-width</td>
   <td>borderLeftWidth</td>
  </tr>
  <tr>
   <td>border-right</td>
   <td>borderRight</td>
  </tr>
  <tr>
   <td>border-right-color</td>
   <td>borderRightColor</td>
  </tr>
  <tr>
   <td>border-right-style</td>
   <td>borderRightStyle</td>
  </tr>
  <tr>
   <td>border-right-width</td>
   <td>borderRightWidth</td>
  </tr>
  <tr>
   <td>border-style</td>
   <td>borderStyle</td>
  </tr>
  <tr>
   <td>border-top</td>
   <td>borderTop</td>
  </tr>
  <tr>
   <td>border-top-color</td>
   <td>borderTopColor</td>
  </tr>
  <tr>
   <td>border-top-style</td>
   <td>borderTopStyle</td>
  </tr>
  <tr>
   <td>border-top-width</td>
   <td>borderTopWidth</td>
  </tr>
  <tr>
   <td>border-width</td>
   <td>borderWidth</td>
  </tr>
  <tr>
   <td>clear</td>
   <td>clear</td>
  </tr>
  <tr>
   <td>clip</td>
   <td>clip</td>
  </tr>
  <tr>
   <td>color</td>
   <td>color</td>
  </tr>
  <tr>
   <td>cursor</td>
   <td>cursor</td>
  </tr>
  <tr>
   <td>display</td>
   <td>display</td>
  </tr>
  <tr>
   <td>filter</td>
   <td>filter</td>
  </tr>
  <tr>
   <td>font</td>
   <td>font</td>
  </tr>
  <tr>
   <td>font-family</td>
   <td>fontFamily</td>
  </tr>
  <tr>
   <td>font-size</td>
   <td>fontSize</td>
  </tr>
  <tr>
   <td>font-variant</td>
   <td>fontVariant</td>
  </tr>
  <tr>
   <td>font-weight</td>
   <td>fontWeight</td>
  </tr>
  <tr>
   <td>height</td>
   <td>height</td>
  </tr>
  <tr>
   <td>left</td>
   <td>left</td>
  </tr>
  <tr>
   <td>letter-spacing</td>
   <td>letterSpacing</td>
  </tr>
  <tr>
   <td>line-height</td>
   <td>lineHeight</td>
  </tr>
  <tr>
   <td>list-style</td>
   <td>listStyle</td>
  </tr>
  <tr>
   <td>list-style-image</td>
   <td>listStyleImage</td>
  </tr>
  <tr>
   <td>list-style-position</td>
   <td>listStylePosition</td>
  </tr>
  <tr>
   <td>list-style-type</td>
   <td>listStyleType</td>
  </tr>
  <tr>
   <td>margin</td>
   <td>margin</td>
  </tr>
  <tr>
   <td>margin-bottom</td>
   <td>marginBottom</td>
  </tr>
  <tr>
   <td>margin-left</td>
   <td>marginLeft</td>
  </tr>
  <tr>
   <td>margin-right</td>
   <td>marginRight</td>
  </tr>
  <tr>
   <td>margin-top</td>
   <td>marginTop</td>
  </tr>
  <tr>
   <td>overflow</td>
   <td>overflow</td>
  </tr>
  <tr>
   <td>padding</td>
   <td>padding</td>
  </tr>
  <tr>
   <td>padding-bottom</td>
   <td>paddingBottom</td>
  </tr>
  <tr>
   <td>padding-left</td>
   <td>paddingLeft</td>
  </tr>
  <tr>
   <td>padding-right</td>
   <td>paddingRight</td>
  </tr>
  <tr>
   <td>padding-top</td>
   <td>paddingTop</td>
  </tr>
  <tr>
   <td>page-break-after</td>
   <td>pageBreakAfter</td>
  </tr>
  <tr>
   <td>page-break-before</td>
   <td>pageBreakBefore</td>
  </tr>
  <tr>
   <td>position</td>
   <td>position</td>
  </tr>
  <tr>
   <td>float</td>
   <td>cssFloat</td>
  </tr>
  <tr>
   <td>text-align</td>
   <td>textAlign</td>
  </tr>
  <tr>
   <td>text-decoration</td>
   <td>textDecoration</td>
  </tr>
  <tr>
   <td>text-decoration: blink</td>
   <td>textDecorationBlink</td>
  </tr>
  <tr>
   <td>text-decoration: line-through</td>
   <td>textDecorationLineThrough</td>
  </tr>
  <tr>
   <td>text-decoration: none</td>
   <td>textDecorationNone</td>
  </tr>
  <tr>
   <td>text-decoration: overline</td>
   <td>textDecorationOverline</td>
  </tr>
  <tr>
   <td>text-decoration: underline</td>
   <td>textDecorationUnderline</td>
  </tr>
  <tr>
   <td>text-indent</td>
   <td>textIndent</td>
  </tr>
  <tr>
   <td>text-transform</td>
   <td>textTransform</td>
  </tr>
  <tr>
   <td>top</td>
   <td>top</td>
  </tr>
  <tr>
   <td>vertical-align</td>
   <td>verticalAlign</td>
  </tr>
  <tr>
   <td>visibility</td>
   <td>visibility</td>
  </tr>
  <tr>
   <td>width</td>
   <td>width</td>
  </tr>
  <tr>
   <td>z-index</td>
   <td>zIndex</td>
  </tr>
 </tbody>
</table>
