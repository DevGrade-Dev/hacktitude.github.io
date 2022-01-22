[<< home](./README.md)

# Challenge 12

After enrolling into a course, the user should be able to `pin` and `unpin` a course. This pinned state should be stored and kept in the Database.

Once this task is complete, the `Enrolled` page should indicate if a particular course is pinned by the user or not as shown below.

<img src="./images/12_1.png" width="400">

## Challenge 12.a [1 Point]

Changing the `pinned` state of a course should be done though the course dashboard page.

<img src="./images/12a1.png " width="400">

Currently, the pin button is shown for all the courses in the `course-dashboard.ejs` page regardless if the user has enrolled or not. You have to fix this and render the element which has the id `pin` only if the user is enrolled to the particular course.

>> NOTE: You must use EJS server scripts for this. (Not client side JavaScript)

## Challenge 12.b [1 Point]

You need a location in the database to keep the pinned state of a course.

For this, you have to add a new column called `pinned` in `userCourses` which should accept boolean (or 1 and 0) values.

>>HINT: Always use `migrate` files to do DB changes. 

>>In `createTable()`statement of the migration file, you can create a boolean column with statement `table.boolean("pinned")` to achieve this.

## Challenge 12.c [6 Points]

<img src="./images/12c1.png" width="400">

On course dashboard, when the pin icon is clicked, `pinned` status should be toggled in the database.

Use `/course/pin/:cid` route in `courseController.js` to implement this without changing the route signature. You will have to implement the logic inside this route.

## Challenge 12.d [1 Point]

Now you need to change the `Enrolled` page so that users are able to see the pinned state of the listed courses.

<img src="./images/12_1.png" width="400">

In `enrolled.ejs`, only the courses that are pinned should render the element starting with id `pin-`. If a course is not pinned, then the element should not be rendered.

>> NOTE: Use EJS server scripts for this. Do not use client side JavaScript.
