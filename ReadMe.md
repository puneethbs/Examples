** HTML 5: **

HTML4(12/1997) --16+ years--> HTML5(10/2014)

HTML5 Features:
- Dynamic Behavior
- New features based on HTML, CSS, DOM and Javascript
- New API: Storage, Geo location, audio-video, web sockets etc
- New markups for data  lists, progress bars, input types
- No more Flash required
- Device independent

Few HTML5 Semantics:
- <section> : Grouping a content with heading
- <nav> : Defines a set of navigation link
- <article> : Specifies independent, self-contained content
- <aside> : Contents related but separate frm main element like side bar
- <hgroup> : H1-H6 elements, used when heading has multiple elements
- <header> : Heading
- <footer> : Footer
- <time> : Machine readable time

Data Attributes:
data-* attributes is used to store custom data private to the page or application
'''html
<ul>
  <li data-animal-type="bird">Owl</li>
  <li data-animal-type="fish">Salmon</li> 
  <li data-animal-type="spider">Tarantula</li> 
</ul>
'''

WebStorage:

- Stores data in key-value pair with in the user browser
- Network-efficient(data is not transmitted), can contain larger data than cookies

 - localStorage:
   - separate storage area for given origin
   - persists data even when the browser is closed and reopened
   - updates are propagated to opened tabs for same origin
   '''javascript
   localStorage.setItem(key, data);
   localStorage.getItem(key);
   localStorage.removeItem(key);
   localStorage.length;
   localStorage.clear();
   '''
 - sessionStorage:
   - separate storage area for given origin
   - only for browser tab session
   - retains data on page refresh
   - updates are not propagated to the opened tabs for same origin
   '''javascript
   sessionStorage.setItem(key, data);
   sessionStorage.getItem(key);
   sessionStorage.removeItem(key);
   sessionStorage.length;
   sessionStorage.clear();
   '''

Application Cache:
- Accessible without internet, work offline
- Speed- loads faster
- Reduces server load

'''html
<html manifest="app.appcache">
---
<html>
'''
'''markdown
CACHE MANIFEST

CACHE: #- Explicitly cached after first load. Default.
styles/style.css
scripts/lib/jquery-1.10.1.min.js
scripts/script.js
images/logo/angularjs_logo.png

NETWORK: #- Never cached. Needs browser to be online
*

FALLBACK: #- fallback pages if a page is inaccessible
/ /offline.html
'''

- HTML 5 Validator: https://html5.validator.nu/
- HTML 5 Minimum MarkUp: http://www.google.com/404
- Live DOM Viewer: http://software.hixie.ch/utilities/js/live-dom-viewer/
- MDN HTML Elements: https://developer.mozilla.org/en-US/docs/Web/HTML/Element
 
