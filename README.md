#Pagemark
Pagemark is a small snippet of code that allows you to "bookmark" locations on a web page and then quickly navigate back to them. Useful for infinite scrolling pages with videos on them (such as a tumblr feed or RSS reader) where you wish to begin to buffer a video, continue scrolling and then return to it later.

## Usage
Copy and paste the following into the URLbar of the page you want to activate Pagemark on.

    javascript: (function() {
       var a = document.createElement("script");
       a.type = "text/javascript";
       a.src = "http://www.kerryck.com/resources/js/pagemark.js";
       document.getElementsByTagName("head")[0].appendChild(a)
    })();

Then, on the web page with pagemark:

1. CTRL+Click to add a scroll location to come back to later. A star should appear below your cursor.
2. Continue scrolling down the page, optionally staring more scroll locations.
3. Use CTRL+Up/Down to jump to each starred scroll location.

## Note
Newer versions of Firefox wont allow bookmarklets ([see issue](https://bugzilla.mozilla.org/show_bug.cgi?id=527530)).
