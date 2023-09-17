1. What tech stack will you use for your final project? We recommend that you use
React and Node for this project, however if you are extremely interested in
becoming a Python developer you are welcome to use Python/Flask for this
project.

React, Node, Express, PostgresQL

2. Is the front-end UI or the back-end going to be the focus of your project? Or are
you going to make an evenly focused full-stack application?

Front end will compose of most of the work. Back end will primarily be set up to be able to CRUD data. 

3. Will this be a website? A mobile app? Something else?

This will be a website but the logic and back-end can be used later to rebuild the app in React Native to transition into a mobile app.

4. What goal will your project be designed to achieve?

The goal is to create a minimalist and simple workout tracker that is easy to navigate with UI elements such as a calendar and uncluttered sidebar. 

5. What kind of users will visit your app? In other words, what is the demographic of
your users?

No particular age group is being targeted but rather people who exercise or work out as a hobby/lifestyle.

6. What data do you plan on using? How are you planning on collecting your data?
You may have not picked your actual API yet, which is fine, just outline what kind
of data you would like it to contain. You are welcome to create your own API and
populate it with data. If you are using a Python/Flask stack are required to create
your own API.

I am creating my own API and populating it with data via inputting into a CSV file for ease of editting and having the database be loaded with data from that CSV.

7. In brief, outline your approach to creating your project (knowing that you may not
know everything in advance and that these details might change later). Answer
questions like the ones below, but feel free to add more information:
- What does your database schema look like?
The database will be comprised of 5 tables:
  - Users: containing usernames and hashed passwords
  - Exercises: supplied by data inputted into our API, consists of name, equipment type, description/instructions and possibly a link to recommended instructional video
  - Templates: a one-to-many relationship table linking templates to multiple exercises
  - Workouts: a one-to-many relationship table linking a workout to multiple exercises including details such as sets, reps, weight, etc. 
  - Tags: a many-to-many relationship table linking exercises to body parts that they train
- What kinds of issues might you run into with your API? This is especially
important if you are creating your own API, web scraping produces
notoriously messy data.
  - Since data is being provided by my own input, there shouldn't be any web scraping issues. Simply setting up the API should be the only obstacle as well as making sure I input data at a reasonable time. 
- Is there any sensitive information you need to secure?
  - None other than simple passwords (hashed).
- What functionality will your app include?
  - A calendar UI to navigate workouts
  - The ability to view workouts you've done before
  - Templates so you can easily structure repeatable workouts
  - Exercise look up
  - Exercise filter by equipment type/body part
- What will the user flow look like?
  - The user will sign up/log on and immediately be able to view the current date's workout. They can navigate through workouts on certain dates with the calendar UI. If they wish to add an exercise to workout, an add-exercise button should direct them towards a search UI that allows them to look and filter through different exercises. Users can also choose to go to a exercise directly and render a more detailed page with description, instructions and possibly a video. 
- What features make your site more than a CRUD app? What are your
stretch goals?
  - Current stretch goals are to create trackers for progress and consistency, taking data for a user and converting it into a visually digestible form. Another is create a program via .csv download/upload, where a user essentially can share templates that correspond to a program and assign it to different days. 
