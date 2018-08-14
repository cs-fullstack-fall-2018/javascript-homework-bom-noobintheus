# javascript-homework-BOM/DOM - Know What You Are Dealing With

## Accommodating Your User's Machine Capabilities

As a web developer, many times it's important that you sniff out every little detail you can about the User's setup before you 
return anything.

- If their monitor resolution is low, your code may choose to return images of some specified depth (monitor width and height) 
- Based on the Color and Pixel depth of their graphics card, you may want to return and image and/or video stream at a particular 
resolution.

For this homework assignment simply write an HTML page with embedded JavaScript that ouputs some of the most important properties of 
the ```screen``` and ```window``` objects available to you as a Developer via the Browser Object Model (BOM). While some flavors of web 
browsers may support extended properties, the properties in this exercise are standard across all current web browsers so use them 
to your advantage.

### Create a basic HTML file and add the JavaScript necessary to display the following key stats about the User session:
HINT: From ```screen``` object:
1. The site visitor's screen: Width
2. The site visitor's screen: Height
3. The site visitor's screen: Available Width
4. The site visitor's screen: Available Height
5. The site visitor's screen: Color Depth
6. The site visitor's screen: Pixel Depth

### To Customize the User's experience and to enforce security measures, you need to understand how to sniff out additional details regarding the source locations/protocols that fed into the document you are presenting to a User. Again, you should use and all technical details available.

HINT: From ```document``` object:

1. Return the hostname and port of the current URL
2. Return the entire URL of the current page
3. Return the path name of the current URL
4. Return the protocol portion of the current URL

==============================================================

All of the above can be easily extracted from the ```screen`` and ```document`` portions of the BOM/DOM.

Display any way you see fit and remember:
* Doesn't always have to be fancy
* You can always just build a String
* When it comes time to display in browser you have to *write* to the document (DOM) not just make a String so 
maybe build the String and then use document.write(whateverYourString) to actually make it display.
* When it comes to building a String that you ultimately will write into the DOM, you absolutely can include 
HTML elements as Strings to make it display properly, or as one property per row. For Example:
```document.write("<h1>Hello World!</h1><p>Have a nice day!</p>");```
