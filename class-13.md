# “The Past, Present, and Future of Local Storage for Web Applications”

- "HTML5 Storage" is named *Web Storage*, which was at one time part of the HTML5 specification proper, but was split onto its own specification. Certain browsers refer to it as "Local Storage" or "DOM Storage". 
- Instead of fulling writing out the function, you can use "Modernizr.localstorage". This will detect support for HTML5 Storage.
- Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the exact same key, also known as a string. It can be supported by JS, including strings, Booleans, integers or floats. The data is actually stored as a string. If you are storing or retrieving anything other than strings, you will need to utilize functions like "parseInt()" or "parseFloat()".
- Calling "setItem()" with a named key that already exists will silently overwrite the previous value. Calling "getItem()" with a non-existent key will return null rather than throw an exception.
- You can treat localStorage object as an associative array. Instead of getItem() and setItem() methods, you can simply use square brackets. 
- There are also methods for removing the value for a given named key and clearing the entire storage area(deleting all keys & values at once)
- Calling "removeItem()" with a non-existent key will do nothing
- Property to get the total number of values in the storage area, and to iterate through all of the keys by index (getting the name of each key). If you were to call "key()" with an index that isn't between 0-(length-1), the function will return as null.
- # Tracking Changes
- *storage event* will keep track programmatically of when the storage area changes. The storage event is fired on the window object whenever "setItem()", "removeItem()", or "clear()" is called and actually changes something. 
- *storage event* is supported everywhere the localStorage object is supported. In order to hook up the storage event, you'll need to check which event mechanism the browser supports. 
# Limitations in Current Browsers
- 5 megabytes is the amount of storage spach each origin gets by default. You're storing strings, not data in its original formal. If you are storing a lot of integers or floats, the difference can add up. Each digit in that float is being stored as a character, not in the of a floating point number.
- "QUOTA_EXCEEDED_ERR" is the exception that will get thrown if you exceed your storage quote of 5 megabytes. 
# Storage in Action:
- With HTML5 storage, we can save the progress locally within the browser itself
