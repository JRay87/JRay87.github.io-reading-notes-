# Day 13 - Local Storage

## *Local Storage for web applications*

Local storage is the web developers solution to the inability for web browsers to store user data such as preferences without slowing down the website by overloading it with cookies. HTML5 was the first to successfully implement a client side storage for data not needing to be sent to the server but persisted after refreshing the page or between visits.

Local storage went through different itterations differing between browsers and amount of data stored. HTML5 wanted to *"provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins."*

First step is to access the HTML5 storage to see whether your browser supports HTML5 with the `localStorage` object

    `function supports_html5_storage() {`
      `try {`
       `return 'localStorage' in window && window['localStorage'] !== null;`
       `} catch (e) {`
    `return false;`
      `}`
    `}`

HTML5 stores its data in the local browser in key/value pairs with both values being stored as a string (so ***remember parseInt etc., if you're needing it in a different format when retreiving***).

`setItem();`(`[]` notation also allowed) allows you to set and overwrite the values stored. You can also clear the object stored properties and to open and expand the stored data in an alphabetized index.

"Trapping" the storage happens when the browser gets a new "snapshot" of the key/value pairs following a change to data stored in the local storage. This is done with the `storage` function(? - was this just the name used for the example?).

HTML5 stores up to 5MB of user data in local storage and (as of 2011) can not be expanded.

## I'd like to know:

What changes have happened since 2011 to HTML5 and local storage?