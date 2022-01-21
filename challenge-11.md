[<< home](./README.md)

# Challenge 11

Currently in the system there is no mechanism to remind users of `inactive` courses. Inactive are the courses to which the user is enrolled to, but not visited for 14 days or more.

<img src="./images/11b1.png" width="400">

## Challenge 11.a [1 Point]

Currently the `last resumed` date of a course is not captured when someone visits a course, Therefore, you have to create a new column in `userCourses` table called `last_resumed_date` to capture this. This column should be able to accept `date` datatype.

>>NOTE: DB changes should be only done through `migrate` files.

After enrolling in a course, when a user clicks on the `Resume Learning` button, the current date should be updated to this new `last_resumed_date` column.

## Challenge 11.b [4 Points]

The `<p>` tag which is in the `enrolled.ejs` with the id starting with `inactive-` should only be rendered if the current date is more than or equal to 14 days since the last resumed date.

>>NOTE: To make it invisible, do NOT use client side JavaScript such as`style='display: none;'`. But use EJS server scripts to not render the `<p>` tag.
