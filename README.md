Assignment 2 - Short Stack: Basic Two-tier Web Application using HTML/CSS/JS and Node.js
===

## To-Do List
My application is a simple to do list / assignment tracker with a progress bar and ability to implement a due date feature. It is a cute pixel style that mimics a game style. When first loading into my application, there will be a sample task displayed, you can delete that and start adding in your own tasks. The progress bar will keep track of the amount of tasks you have left to complete and will celebrate when you complete all of them correctly! The CSS positioning I used was mainly a CSS flexboxes. I used the main.css file for a majority of my styling, but for inline editing and the confetti I supplemented within main.js client side to properly format those extra features. 

Render Link:
https://a2-amandalongo-a25.onrender.com/

## Technical Achievements
- **Tech Achievement 1**: Using a combination of CSS Selector Functionality
- CSS is organized in an external stylesheet (`main.css`) and uses flexbox for layout, custom fonts from Google Fonts, and a variety of selectors for styling different elements and states. I also used Awesome Fonts for different icons
- **Tech Achievement 2**: One HTML Form, results and validation
- The application uses a single HTML form for adding new tasks, with client-side validation to prevent empty submissions. The form includes a text input for the task and a date input for the due date.
<img width="1512" height="749" alt="Screenshot 2025-09-10 at 7 41 00 PM" src="https://github.com/user-attachments/assets/743192cb-e18f-434d-9916-286ed18528f9" />
- All tasks are displayed in a dynamic, live-updating list on the main page. The list is fetched from the server using JavaScript and updated whenever tasks are added, edited, or deleted.
- **Tech Achievement 3**: Ability to modify existing data
- Users can edit existing tasks and due dates directly in the UI using inline editing. When a task is edited, the changes are sent to the server and the updated dataset is returned and rendered immediately.
- **Tech Achievement 4**: Implemented all necessary/required functionalities
- The server maintains a tabular dataset of tasks, each with fields for task name, creation date, due date, completion status, and a derived field for days until due. This dataset is stored in memory and updated in real time.
- Tasks can be deleted with a single click, and the UI updates instantly to reflect the change. The server removes the task from its dataset and returns the new list.
- **Tech Achievement 5**: Due in ___ days feature using derived field 
- The derived field is displayed in the UI as "Due in X days", "Due today", or "Overdue by X days", depending on the value. This provides clear feedback to users about upcoming and overdue tasks. 
- The server logic includes a function to compute a derived field (`days_until_due`) for each task, based on the due date and current date. This field is recalculated every time the dataset is updated.
- This was specifically difficult because calculating Days Until Due within the server size was giving me wrong timing and wasn't super accurate with what I ended up finding because of my testers. I think I had issues with the timing and when exactly things were due especially since time is a factor when it comes to due dates. I would have liked to have spent more time researching and figuring out how to get past this problem, but I ran out of time since I did my testing so late. 
- **Tech Achievement 6**: Progress Tracker 
- The progress bar at the top of the app visually tracks the number of completed tasks versus total tasks. When all tasks are completed, a confetti animation celebrates the achievement.

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
