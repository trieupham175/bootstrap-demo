# Javascript with Bootstrap

## jQuery - the old friend
### Advantages
- Easy to use
- Includes many utils function: parse data, string strim, array search...
- Cross-browser compatible
- Great community supports.
- Good documentation

### Downloads
- Using `npm`
- Using `CDN distribution`

## Query elements
### document.getElementById
#### Example
Given a HTML document:
```html
<html>
    <body>
        <div id="my-carousel">
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>        
        </div>    
    </body>
</html>
```
The script below will return the DOM of `my-carousel` wrapper div.
```js
var element = document.getElementById('my-carousel');
/** return DOMElement<div>*/
```

#### Parameters
- `id`: `string`. ID of the Element (case-sensitive)

#### Return
- `Element` | `null`. A DOM Element if found  

### document.getElementsByClass
#### Example
Given a HTML document:
```html
<html>
    <body>
        <div id="my-carousel">
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>        
        </div>    
    </body>
</html>
```
The script below will return the DOMs of `carousel-item` wrapper div.
```js
var element = document.getElementsByClassName('carousel-item');
/** return HTMLCollection[3][...]*/
```

#### Parameters
- `className`: `string`. Class name of the elements (case-sensitive)
#### Return
- `HTMLCollection` | `null`. A DOM `array-like` data structures that contains multiple DOM elements

### document.querySelector
#### Example
```html
<html>
    <body>
        <div id="my-carousel">
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>        
        </div>    
    </body>
</html>
```

Instead of using `document.getElementById`, we can use `document.querySelector`

```js
// return the div#my-carousel
var carousel = document.querySelector('#my-carousel');
// return the first div.carousel-item
var carouselItem = document.querySelector('.carousel-item');
```

#### Parameters
- `selectors`: Multiple [CSS Selector](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors)

#### Return value
- `Node` | `null`: the first element that matches if found.

### document.querySelectorAll
#### Example
```html
<html>
    <body>
        <div id="my-carousel">
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>
            <div class="carousel-item"></div>        
        </div>    
    </body>
</html>
```
Instead of using `document.getElementsByClassName`, we can use `document.querySelectorAll`

```js
// return all div.carousel-item
var carouselItems = document.querySelectorAll('.carousel-item');
```

## Set attributes
### Element.setAttribute
#### Parameters
- `name`: `string`. Specific attribute whose value is to be set.
- `value`: `any`. The value that assign to the attribute.
#### Return value
This APi return `undefined`.

## Glossary

### JS Event Delegation
- [Explanation - Read more](https://viblo.asia/p/event-delegation-in-javascript-V3m5WALEZO7)
### Web API
- [document.getElementById](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById)
- [document.getElementsByClassName](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByClassName)
- [document.querySelector](https://developer.mozilla.org/en-US/docs/Web/API/Element/querySelector)
- [document.querySelectorAll](https://developer.mozilla.org/en-US/docs/Web/API/Element/querySelectorAll)
- [Element.setAttribute](https://developer.mozilla.org/en-US/docs/Web/API/Element/setAttribute)

## [Git] Solve the conflicts. 
