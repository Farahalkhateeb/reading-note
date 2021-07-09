# What is localStorage in JavaScript?
localStorage is a property that allows JavaScript sites and apps to save key-value pairs in a web browser with no expiration date. This means the data stored in the browser will persist even after the browser window is closed.





# 



# Where is localStorage stored?
In Google Chrome, web storage data is saved in an SQLite file in a subfolder in the user’s profile. The subfolder is located at \AppData\Local\Google\Chrome\User Data\Default\Local Storage on Windows machines and ~/Library/Application Support/Google/Chrome/Default/Local Storage on macOS

Firefox saves storage objects in an SQLite file called webappsstore.sqlite, which is also located in the user’s profile folder.

 # What is Window.localStorage?
The localStorage mechanism is available via the Window.localStorage property. Window.localStorage is part of the Window interface in JavaScript, which represents a window containing a DOM document.

The Window interface features a wide range of functions, constructors, objects, and namespaces. Window.localStorage is a read-only property that returns a reference to the local storage object used to store data that is only accessible to the origin that created it.

How does localStorage work?
To use localStorage in your web applications, there are five methods to choose from:

setItem(): Add key and value to localStorage
getItem(): This is how you get items from localStorage
removeItem(): Remove an item by key from localStorage
clear(): Clear all localStorage
key(): Passed a number to retrieve the key of a localStorage
setItem(): How to store values in localStorage
Just as the name implies, this method allows you to store values in the localStorage object.

It takes two parameters: a key and a value. The key can be referenced later to fetch the value attached to it.

window.localStorage.setItem('name', 'Obaseki Nosa');
Where name is the key and Obaseki Nosa is the value. Also note that localStorage can only store strings.

To store arrays or objects, you would have to convert them to strings.

To do this, we use the JSON.stringify() method before passing to setItem().

const person = {
    name: "Obaseki Nosa",
    location: "Lagos",
}

window.localStorage.setItem('user', JSON.stringify(person));
getItem(): How to get items from localStorage
To get items from localStorage, use the getItem() method. getItem() allows you to access the data stored in the browser’s localStorage object.

getItem() accepts only one parameter, which is the key, and returns the value as a string.

To retrieve a user key:

window.localStorage.getItem('user');
This returns a string with value as:

“{“name”:”Obaseki Nosa”,”location”:”Lagos”}”
To use this value, you would have to convert it back to an object.

To do this, we make use of the JSON.parse() method, which converts a JSON string into a JavaScript object.

JSON.parse(window.localStorage.getItem('user'));
removeItem(): How to delete localStorage sessions
To delete local storage sessions, use the removeItem() method.

When passed a key name, the removeItem() method removes that key from the storage if it exists. If there is no item associated with the given key, this method will do nothing.

window.localStorage.removeItem('name');
clear(): How to delete all items in localStorage
Use the clear() method to delete all items in localStorage.

This method, when invoked, clears the entire storage of all records for that domain. It does not receive any parameters.

window.localStorage.clear();
key(): How to get the name of a key in localStorage
The key() method comes in handy in situations where you need to loop through keys and allows you to pass a number or index to localStorage to retrieve the name of the key.

var KeyName = window.localStorage.key(index);
localStorage browser support
localStorage as a type of web storage is an HTML5 specification. It is supported by major browsers including IE8. To be sure the browser supports localStorage, you can check using the following snippet:

if (typeof(Storage) !== "undefined") {
    // Code for localStorage
    } else {
    // No web storage Support.
}
localStorage limitations
As easy as it is to use localStorage, it is also easy to misuse it. The following are limitations, and also ways to NOT use localStorage:

Do not store sensitive user information in localStorage
It is not a substitute for a server based database as information is only stored on the browser
localStorage is limited to 5MB across all major browsers
localStorage is quite insecure as it has no form of data protection and can be accessed by any code on your web page
localStorage is synchronous, meaning each operation called would only execute one after the other
With these, we have been armed with the power of localStorage in our web applications.

LogRocket: Debug JavaScript errors easier by understanding the context
Debugging code is always a tedious task. But the more you understand your errors the easier it is to fix them.

LogRocket allows you to understand these errors in new and unique ways. Our frontend monitoring solution tracks user engagement with your JavaScript frontends to give you the ability to find out exactly what the user did that led to an error.

![local storege](https://res.cloudinary.com/practicaldev/image/fetch/s--WSpOuQ_Q--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/zy4kwztfmkw5lb4cjpdz.png)