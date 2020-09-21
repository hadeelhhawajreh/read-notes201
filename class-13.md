Read: 13 - Local Storage

INTRODUCING HTML5 STORAGE
What I will refer to as “HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.

So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

check for HTML5 Storage


``function supports_html5_storage() {``
  ``try {``
    ``return 'localStorage' in window && window['localStorage'] !== null;``
  ``} catch (e) {``
    ``return false;``
  ``}``
``}``

**Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage.**

``if (Modernizr.localstorage) {// window.localStorage is available!``
``} else {``
  ``// no native support for HTML5 storage :(``
  ``// maybe try dojox.storage or a third-party solution``
``}``


USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};
Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.

Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets. For example, this snippet of code:

var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
…could be rewritten to use square bracket syntax instead:

``var foo = localStorage["bar"];``

``localStorage["bar"] = foo;``
There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).

``interface Storage {``
  ``deleter void removeItem(in DOMString key);``
  ``void clear();``
``};``

Calling ``removeItem() ``with a non-existent key will do nothing.

Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).

``interface Storage {``
  ``readonly attribute unsigned long length;``
  ``getter DOMString key(in unsigned long index);``
``};``
If you call ``key() ``with an index that is not between 0–(length-1), the function will return null.

