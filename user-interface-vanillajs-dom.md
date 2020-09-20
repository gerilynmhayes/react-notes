# My Notes on React

Tuesday, September 8, 2020

## A Beginner's Guide to React Introduction

[GitHub repo from Kent C. Dodds](https://github.com/kentcdodds/beginners-guide-to-react/tree/egghead)

Refer to Kent's [Uses Page](https://kentcdodds.com/uses/) to set up your build environment like his; will make following along after watching the tutorial in its entirety.

### Create a User Interface with Vanilla JavaScript and DOM

In this video, Kent shows us the necessary code to create the user interface. He tells us that we're going to need to append our JavaScript DOM (Document Object Model) elements, which will be the `root` of our application.

Then, we'll need to get access to the JS DOM element using the document's API. 

Note: The *definition of an API*, according to Wikipedia:

> An application programming interface is a computing interface which defines interactions between multiple software intermediaries. It defines the kinds of calls or requests that can be made, how to make them, the data formats that should be used, the conventions to follow, etc. It can also provide extension mechanisms so that users can extend existing functionality in various ways and to varying degrees. An API can be entirely custom, specific to a component, or it can be designed based on an industry-standard to ensure interoperability. Through information hiding, APIs enable modular programming, which allows users to use the interface independently of the implementation. [Wikipedia](https://en.wikipedia.org/wiki/API)

From here, we will create the element and add properties to it. Then we'll append it to the DOM element.

Below is the code Kent writes out for us in the tutorial. Review it alongside the tutorial video before moving forward:

```
<body>
  <div id="root"></div>
  <script type="text/javascript">
    const rootElement = document.getElementById('root');
    const element = document.createElement('div');
    element.textContent = 'Hello World';
    element.className = 'container';
    rootElement.appendChild(element);
  </script>
</body>
```

Review this egghead tutorial about the DOM [here](https://egghead.io/lessons/javascript-wtf-is-the-dom?pl=introduction-to-client-side-web-apis-72d0).