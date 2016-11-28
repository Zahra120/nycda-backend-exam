## NYCDA Backend Exam - Part 2

Given that we have a "customer" resource/model in our web server,

1 - How would you design the routes of your server based on REST convention? List them with VERB and /route

/movies              index.pug
/movies/:id           show.pug
/movies/new           new.pug
/movies/:id/edit      edit.pug

2 - Which pages would require templates, and how would you name them? List them with /route and template-name.extension

index.js

views/movies/index.pug
views/movies/show.pug
views/movies/new.pug
views/movies/edit.pug



=========

3 - What is a database constraint? Name the 3 types of database constraints you have learned.
we define a limitation for the column in database.
unique: true or false, not null: true or false, not empty :true or false



4 - What is a foreign key? Given that you have a Factory that has many cars and car that belongs to a factory, What would be your foreign key column?

-it is column that we put in the table to make a relationship with the other tables.
-the relationship is one to many ,
the foreign key will be carId in the factory table.


5 - List all the model lifecycle hooks you have learned from sequelize and explain them briefly if necessary.

before validate
after validate
before create
after create
before update
after update
before destroy
after destroy

(It will be Great if you explain the hook again. I am not good in it.)



6 - What is the difference between database-level validations and application-level validations?

database-level validation , we put the validation in the database and in the migration files  and when we create the tables. like defining constrains for columns.
application-level validations, we put validate property to do this validation in model part.
we use standard of sequelize in our project. validate: {
                                                          isEmail: true
                                                        } will check the email format.

7 - Why do we use bcrypt. Write down 3 reasons why we use it if you can.
to produce a very secured password that can not be hacked.


8 - What is a flash message?
They are the pop up windows , which we use for application-level validations.

9 - What is the difference between minifying and obfuscating JavaScript?
minify, eliminate all white-spaces from files. obfuscating, changes  variables names to shorter one.

10 - What are the 3 reasons that makes Gulp a good choice as an asset build library?

it uses streams
we can use the ready packages with that, and we don't need to write them by ourselves.
compile scss
watching the changes
