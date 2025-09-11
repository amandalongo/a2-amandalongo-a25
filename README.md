Assignment 2 - Short Stack: Basic Two-tier Web Application using HTML/CSS/JS and Node.js  
===

- a `Server` which not only serves files, but also maintains a tabular dataset with 3 or more fields related to your application
- a `Results` functionality which shows the entire dataset residing in the server's memory
- a `Form/Entry` functionality which allows a user to add or delete data items residing in the server's memory
- a `Server Logic` which, upon receiving new or modified "incoming" data, includes and uses a function that adds at least one additional derived field to this incoming data before integrating it with the existing dataset
- the `Derived field` for a new row of data must be computed based on fields already existing in the row. 
For example, a `todo` dataset with `task`, `priority`, and `creation_date` may generate a new field `deadline` by looking at `creation_date` and `priority`

Your application is required to demonstrate the use of the following concepts:

HTML (4 pts each, total 16 pts):
- One or more [HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms), with any combination of form tags appropriate for the user input portion of the application
- A results page displaying all data currently available on the server. You will most likely use a `<table>` tag for this, but `<ul>` or `<ol>` could also work and might be simpler to work with. Alternatively, you can create a single-page app (see Technical Acheivements) but this is not a requirement.
- All pages should [validate](https://validator.w3.org)
- If your app contains multple pages, they should all be accessible from the homepage (index.html)

CSS (4 pts each, total 16 pts):
- CSS styling of the primary visual elements in the application
- Various CSS Selector functionality must be demonstrated:
    - Element selectors
    - ID selectors
    - Class selectors
- CSS positioning and styling of the primary visual elements in the application:
    - Use of either a CSS grid or flexbox for layout
    - Rules defining fonts for all text used; no default fonts! Be sure to use a web safe font or a font from a web service like [Google Fonts](http://fonts.google.com/)
- CSS defined in a maintainable, readable form, in external stylesheets 

JavaScript (4 pts):
- At minimum, a small amount of front-end JavaScript to get / fetch data from the server; a sample is provided in this repository.

Node.js (4 pts):
- An HTTP Server that delivers all necessary files and data for the application, and also creates the required `Derived Fields` in your data. 
A starting point is provided in this repository.


Acheivements
---

Below are suggested technical and design achievements. You can use these to help customize the assignment to your personal interests. These are recommended acheivements, but feel free to create/implement your own... just make sure you thoroughly describe what you did in your README and why it was challenging. ALL ACHIEVEMENTS MUST BE DESCRIBED IN YOUR README IN ORDER TO GET CREDIT FOR THEM. Remember, the highest grade you can get on any individual assignment is a 100%.

*Technical*
- (5 points) Create a single-page app that both provides a form for users to submit data and always shows the current state of the server-side data. To put it another way, when the user submits data, the server should respond sending back the updated data (including the derived field calculated on the server) and the client should then update its data display.

- (5 points) In addition to a form enabling adding and deleting data on the server, also add the ability to modify existing data.


## To-Do List
My application is a simple to do list / assignment tracker with a progress bar and ability to implement a due date feature. It is a cute pixel style that mimics a game style. When first loading into my application, there will be a sample task displayed, you can delete that and start adding in your own tasks. The progress bar will keep track of the amount of tasks you have left to complete and will celebrate when you complete all of them correctly! The CSS positioning I used was mainly a CSS grid. I used the main.css file for a majority of my styling, but for inline editing and the confetti I supplemented within main.js client side to properly format those extra features. 
https://a2-amandalongo-a25.onrender.com/

## Technical Achievements
- **Tech Achievement 1**: Using a combination of CSS Selector Functionality
- **Tech Achievement 2**: One HTML Form, results and validation
- **Tech Achievement 3**: Ability to modify existing data
- **Tech Achievement 4**: Implemented all necessary/required functionalities
- **Tech Achievement 5**: Due in ___ days feature using derived field 

### Design/Evaluation Achievements
- **Design Achievement 1**:
1. Syed
2. The first tester had issues regarding the font and the lack of features on the application
3. He thought for his purposes of using the application he wouldn't use the date deadline feature. He would just hit enter after writing in a task so it wouldnt have a due date. Which was fine but he thought that it was a pain
4. I would change the font for at least the time feature, because he said it was hard to read the numbers but the whole aesthetic and style of the application was supposed to be pixelated. 

- **Design Achievement 2**:
1. Ramirez
2. He noticed an issue with the date due functionality, specifically the "due in __ days" feature. When he tested it he put the due date to the next day but then the feature calculated it to say "due today" when in reality it was due the next day. 
3. He said he would definitely use this app, especially if it was integrated with canvas assignment tracking. He liked the edit feature and the celebration when you complete all your tasks. He also appreciated the UI. I also noticed he would try to click the progress bar to see if it did anything
4. I would definitely make changes to the due date feature because that was one of the things i had trouble implementing correctly.  
