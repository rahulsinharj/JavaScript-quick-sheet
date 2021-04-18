## Document Object Model:
  * Every web page resides inside a browser window, which can be considered as an object. 
  * A DOM represents the HTML document that is displayed in that window. 
  * The DOM is a tree-like representation of the contents of a webpage. Tree of “nodes” with different relationships depending on how they are arranged in the HTML document.
  * The Document object has various properties that allow access to and modification of document content. 

   ### DOM Properties:
   * With the Document Object Model (DOM), we can create and build documents, add, modify, or delete elements and content.
   * The syntax for accessing the DOM properties is: `document.property_name`.
   * Some most common properties are:
  
   | Property | Description |
   |----------|-------------|
   |document.anchors|It will return all <a> elements that have a name attribute.|
   |document.baseURI|It will return the absolute base URI of the document.|
   |document.body|It will return the <body> element.|
   |document.cookie|It will return the document's cookie.|
   |document.doctype|It will return the document's doctype.|
   |document.documentElement|It will return the <html> element.|
   |document.documentMode|It will return the mode used by the browser.|
   |document.documentURI|It will return the URI of the document.|
   |document.embeds|It will return all HTML <embed> elements.|
   |document.forms|It will return all HTML <form> elements.|
   |document.head|It will return the HTML <head> element.|
   |document.images|It will return all HTML <img> elements.|
   |document.implementation|It will return the DOM implementation.|
   |document.links|It will return all HTML <area> and <a> elements having href attribute.|
   |document.scripts|It will return all HTML <script> elements.|
   |document.title|It will return the <title> element.|
   |document.URL|It will return the complete URL of the document.|

### DOM Selectors:
  * DOM Selectors is used to select HTML elements within a document using JavaScript. 
  * There are two types of a selector, i.e., single element selector and multiple element selector. 
  * Some of the common ways of selecting the elements on a page using different methods are:

  |Gets|Method|Type|
  |----|------|----|
  |ID|getElementById()|Single Element|
  |Class|getElementsByClassName()|Multiple Element|
  |Tag|getElementsByTagName()|Multiple Element|
  |Selector (single)|querySelector()|Single Element|
  |Selector (all)|querySelectorAll()|Multiple Element|


### DOM traversal properties and methods:
  * We can traverse the DOM in three directions, downwards, upwards and sideways. Each type of traversal uses a different method.
  * 
