# Hausaufgabe 08
### Aufgabe 01

> Typen von Knoten in HTML MDN Referenz

[MDN Referenz](https://developer.mozilla.org/en-US/docs/Web/API/Node#Properties)

### querySelector, querySelectorAll und getElementBy...

1. querySelector
    
    - gibt uns das <span style="color:red">erste</span> Element das wir suchen
    - Schreibweise wie jQuery

```javascript
document.querySelector("h2") // element h2
document.querySelector("#title") // element mit id title
document.querySelector(".title") // element mit klasse title 
element.querySelector(".title") // element mit klasse title innerhalb von elemennt
document.querySelector("p.example") // Get the first <p> element in the document with class="example"
document.querySelector("div > p") // Get the first <p> element in the document where the parent is a <div> element
document.querySelector("a[target]") // Get the first <a> element in the document that has a "target" attribute
document.querySelector("h2, h3").style.backgroundColor = "red"
``` 

[querySelector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)

2. querySelectorAll

    - gibt uns ein Array mit <span style="color:red">allen</span> Elementen die wir suchen
    - Schreibweise wie in jQuery

```javascript
document.querySelectorAll("h2") // alle elemente h2
document.querySelectorAll("#title") // alle elemente mit id title
document.querySelectorAll(".title") // alle elemente mit klasse title
document.querySelectorAll(".title")[0] // erstes element mit klasse title (wie document.querySelector(".title"))
```  

[querySelectorAll](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelectorAll)

3. getElementBy...

```javascript
document.getElementById("identity") // element mit id ...
document.getElementsByClassName("klasse") // array mit elemente mit klasse ...
``` 

[getElement...](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById)

### Aufgabe 03

