# Forms

Last week you made a simple form using React components.  This form doesn't
post to anywhere yet, we'll be doing that today!

## High Level Overview
* Web applications usually have to communicate with servers
* Using AJAX (Asyncronous Javascript and XML), you can make a request to the server
  and the server will send back a response that you can then display on the
  same page without refreshing the page.
* You can read more about AJAX online
* You send information to and from servers in the form of a JSON object (basically
  a dictionary)
  * You do this in 168 and also in internships! *cue Julia's internship video*

## Superagent
* We will be using the [Superagent API](https://visionmedia.github.io/superagent/)
  for our requests!  The documentation is really good, so make sure to read through
  it thoroughly.
* To include it in your react app, run `yarn add superagent` and then `import request
  from 'superagent'` at the top of your file.
* You will be posting to a server hosted on Christian's website, details below.

## Web Tier Server API
* The server is located at `http://webtier.christianle.com/v1/contact`.
* The server takes in the following:
  * `first`: a string that is the first name from the form
  * `last`: a string that is the last name from the form
  * `email`: a string that is the email from the form
  * `phone`: a string that is the phone number from the form
* You should be creating a JSON object to send all of these items to the server
* You can handle error/success however you want.  In my example, I simply
  printed the response message from the server to the screen.

## Dealing with APIs you didn't write
* When you receive something back from the server, you can look at the object
  you got back with `console.info(Object.keys(err))` or `console.info(Object.keys(res))`
* You can then go into your console and look at the JSON object to determine
  things such as the status code, or the error message the server sends back
* Example: In errors I handle 400 and 500 errors (bad params and general server
  error) by printing out the message from the server for both errors but 
  also listing out which params were bad/missing for the 400 error.  I got this
  information by using `console.log` to figure out what kind of information the
  server was sending back to me.
