## NYCDA Backend Exam - Part 3

### 1 - What is the difference between git pull and git merge?

with git pull we can have the changes in the working branch

with git merge we can merge one branch to master, when have done with the project.

### 2 - Why do we use a pull request on github instead of merging our branch directly to master and then pushing it to github?
because like that working on the project will be more organized and we can have different branch for different part of project. Furthermore in the group projects which many people work on the same project and there is only one repo . So it will be easy to have different branches and push the changes to different branches and other persons pull the changes and after everything is complete they can merge the branches to master.

### 3 - Why do we use database migrations?

to transfer the changes we want to do for the database. like adding new column to database

### 4 - What is the difference between up and down functions of sequelize migration files?
we put the changes we want to do on database on up
and we revert that changes in down.
for example:
we put the addColumn in up and we put removeColumn in down part.

### 5 - Name 3 reasons why Sass/SCSS is better than CSS?

we can reuse the styles
it is more readable
 with that, we can split the CSS into smaller parts and then with @import use those parts in the project. like that , the file will be  more maintable.


### 6 - What is the right way to include bootstrap to your project?
we can install the npm package of bootstrap and have locally in hard . and put it in public/vendor folder.

### 7 - Why _variables.scss file is important?

in this file , we have all the styles of variables for the entire project.

### 8 - Lets say you want to change the alert component of bootstrap, what are steps/strategy would you use to make that change?

in the bootstrap folder, we put the _alert.scss
and we put the our styles in the bottom of that file and in the_bootstrap.scss file we include @import "bootstrap/alert";
