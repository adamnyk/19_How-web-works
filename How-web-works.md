# How Web Works Exercise

## Part One: Solidify Terminology
In your own terms, define the following terms:

- What is HTTP?
    Hypertext Transfer Protocol. The standard web protocol for communication between browsers and servers

- What is a URL?
    Uniform resource locator. It is the address to a particular internet resource
    
- What is DNS?
    Domain name server. It is responsible for retrieving IP address from URL names

- What is a query string?
    It provides extra information, such as search terms, info from forms, etc to the server to change the page.  It is located in / at the end of the URL and can be used to input multiple arguments and key value pairs.

- What are two HTTP verbs and how are they different?
    **GET**: is a method to request a URL resource. It is a request that does not change any server data
    **POST**: is a request that does change data on the server / side-effect 

- What is an HTTP request?
    A request from the client to a server with the HTTP protocol. It requests for HTML and website data from the server.

- What is an HTTP response?
    What the server sends back from an HTTP requests, like HTML, JS, CSS.

- What is an HTTP header? Give a couple examples of request and response headers you have seen.
    Headers hold additional information about a server request or response.  
    Examples...
    Request headers: Host, User-Agent, Accept, Cookie, Cache-Control
    Response headers: Content-Type, Last-Modified, Set-Cookie, Cache-Control

- What are the processes that happen when you type “http://somesite.com/some/page.html” into a browser?
    1. Browser converts url into ip address using DNS
    2. Browser makes a request to that IP address with headers
    3. Server sends a response with a status code
    4. Browser makes a DOM (document object model) from the returned HTML & locates other resources that are needed (images, CSS, JS, others)
    5. Browser makes separate HTTP requests for those resources and receives a server response for each


    

________

Part Two: Practice Tools
Using curl, make a GET request to the icanhazdadjoke.com API to find all jokes involving the word “pirate”
Use dig to find what the IP address is for icanhazdadjoke.com
Make a simple web page and serve it using python3 -m http.server. Visit the page in a browser.
Part Three: Explore Dev Tools
Build a very simple HTML form that uses the GET method (it can use the same page URL for the action) when the form is submitted.

Add a field or two to the form and, after submitting it, explore in Chrome Developer tools how you can view the request and response headers.

Edit the page to change the form type to POST, refresh in the browser and re-submit. Do you still see the field in the query string? Explore in Chrome how you can view the request and response headers, as well as the form data.

Part Four: Explore the URL API
At times, it’s useful for your JavaScript to look at the URL of the browser window and change how the script works depending on parts of that (particularly the query string).

Read about the URL API

Try some of the code examples in the Chrome Console so that you can get comfortable with the basic methods and properties for instances of the URL class.

Solution
You can view our solution