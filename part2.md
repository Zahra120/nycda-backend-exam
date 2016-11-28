## NYCDA Backend Exam - Part 2

Given that we have a "customer" resource/model in our web server,

1 - How would you design the routes of your server based on REST convention? List them with VERB and /route

/movies              
/movies/:id         
/movies/new           
/movies/:id/edit      

2 - Which pages would require templates, and how would you name them? List them with /route and template-name.extension
actually I did not get completely, what do you want in this example. It is not clear for me.

index.js

/movies              
/movies/:id         
/movies/new           
/movies/:id/edit   


=========

3 - What is a database constraint? Name the 3 types of database constraints you have learned.
we define a limitation for the column in database.
unique: true or false, not null: true or false, foreign key



4 - What is a foreign key? Given that you have a Factory that has many cars and car that belongs to a factory, What would be your foreign key column?

-  It is used to link two tables and it is a column , we put in one of the table that its value matches with the primary key of the other table.
the foreign key will be factoryId in the Cars table.


5 - List all the model lifecycle hooks you have learned from sequelize and explain them briefly if necessary.

before validate
after validate
before create
after create
before update
after update
before destroy
after destroy
- for example , we can  put a slug for posts if they don't have one, after create  the post.

(It will be Great if you explain the hook again. I am not good in it.)



6 - What is the difference between database-level validations and application-level validations?

database-level validation , we put the validation in the database and in the migration files  and when we create the tables. like defining constrains for columns.
application-level validations, we put validate property to do this validation in model part.
we use standard of sequelize in our project. validate: {
                                                          isEmail: true
                                                        } will check the email format.

7 - Why do we use bcrypt. Write down 3 reasons why we use it if you can.

to produce a very secured password that can not be hacked.
it is a method of crypt package.
it uses a very complicated algoritm to create hash.



8 - What is a flash message?
They are notification messages , to show users that an action was successful or was wrong.
for example if we put correct format of email.

9 - What is the difference between minifying and obfuscating JavaScript?
minify, eliminate all white-spaces from files. obfuscating, changes  variables names to shorter one.

10 - What are the 3 reasons that makes Gulp a good choice as an asset build library?

it uses streams
we can use the ready packages with that, and we don't need to write them by ourselves.
compile scss
watching the changes
