## NYCDA Backend Exam
=====================
Explain the questions well!!

### 1- Why do we should include script tags at the very end of an html file, before closing </body>?

because like that the page will be loaded faster and we can first see the page and we
don't need  to wait for loading script file, because we don't need it at the first
place , we need it , when we interact with the page.

### 2 - What is a middleware?
it is a function that runs before handelers has access to request and response.

### 3 - Why do we use express.static() middleware?
to be able for using static files like css and js and images in our projects, we create a folder named public and we put these files in it. after that we can use these file by
writing this code app.use(express.static('public')) .

### 4 - What is favicon.ico ?
it is the icon that we can see  in  top, next to title of html page in browser,
and we can recognize easily which website , we want to see.

### 5 - Why do we use a bodyParser middleware ?
when we send something to server
through the form , to make it  readable for server we use middleware and it will be saved in req.body object.

### 6 - What is the difference in terms of parsing a data received from a web form with POST or an AJAX POST request?


### 7 - Why do we use methodOverride middleware ?
because the form html by default , doesn't accept put action and delete action, we use this middleware, to make put and delete works on the form.

### 8 - What are the differences between sessions and cookies ?
session is a object that has placed in server  and each session has an unique id that has saved in cookies.
cookie is a string that saved in the browser. both have information about the user saved in them.

### 9 - Why do we use a session middleware ?  
to be able to use easily  session instance in our project . through that we use req.session.user  to put the authentication in our project. if the user loged in we put that user in req.session.user, so req.session.user will hold a truthy value but if we
put undefined in req.session.user  so means the session is over and the user is loged out.

### 10 - Why do we use a build process ?
we use it to make our project more optimized and only have one file for css and another file for script. and that files are minified .like that our project runs very fast.
we use gulp as a build process. because it is easy to use and it compiles scss, it combines files and watches files. it has many packages that we can use and we don't need to write by ourselves.
