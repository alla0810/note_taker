# note_taker
  * Author: Kyosook Shin
  * Author's Email: kyosook.shin@gmail.com  
  * GitHub: https://github.com/alla0810/note_taker
  * Heroku deploy: https://note-taker-for-you-081d407650f3.herokuapp.com/
  * screenshot  

<img src='./public/assets/images/screen1.png' width="600">  
<img src='./public/assets/images/screen2.png' width="600">



## Source Code References
  This project has used some reference codes from the following sites

   * https://git.bootcampcontent.com/University-of-Texas-at-Austin/UTA-VIRT-FSF-PT-07-2023-U-LOLC.git   

   
## User Story

AS a small business owner
I WANT to be able to write and save notes
SO THAT I can organize my thoughts and keep track of tasks I need to complete


## Acceptance Criteria

GIVEN a note-taking application

* WHEN I open the Note Taker, THEN I am presented with a landing page with a link to a notes page

* WHEN I click on the link to the notes page, THEN I am presented with a page with existing notes listed in the left-hand column, plus empty fields to enter a new note title and the note's text in the right-hand column

* WHEN I enter a new note title and the note's text, THEN a "Save Note" button and a "Clear Form" Button appear in the navigation at the top of the page

* WHEN I click on the Save button, THEN the new note I have entered is saved and appears in the left-hand column with the other existing notes and the buttons in the navigation disappear

* WHEN I click on an existing note in the list in the left-hand column, THEN that note appears in the right-hand column and a "New Note" button appears in the navigation

* WHEN I click on the "New Note" button in the navigation at the top of the page, THEN I am presented with empty fields to enter a new note title and the note's text in the right-hand column and the button disappears


## Mock-Up
The following animation shows the web application's appearance and functionality

<img src='./public/assets/images/11-express-homework-demo.gif' width="600" >

## Getting Started
The application should have a `db.json` file on the back end that will be used to store and retrieve notes using the `fs` module. 
The following HTML routes should be created:
* `GET /notes` should return the `notes.html` file.
* `GET *` should return the `index.html` file.

The following API routes should be created:
* `GET /api/notes` should read the `db.json` file and return all saved notes as JSON.
* `POST /api/notes` should receive a new note to save on the request body, add it to the `db.json`file, and then return the new note to the client.  You'll need to find a way to give each note a unique id when it's saved (look into `npm` packages that could do this for you).

## Bonus
You haven't learned how to handle DELETE requests, but this application has that functionality in the front end.  As a bonus, see if you can add the DELETE route to the application using the following guideline:
* `DELETE /api/notes/:id` should receive a query parameter containing the id of a note to delete.  In order to delete a note, you'll need all notes from the `db.json` file, remove the note with the given `id` property, and then rewrite the notes to the `db.json` file.


## Technical Acceptance Criteria: 40%
* Satisfies all of the preceding acceptance criteria plus the following:
  * Application front end must connect to an Express.js back end.
  * Application back end must store notes with unique IDs in a JSON file.
  * Application must be deployed to Heroku.

## Deployment: 36%
* Application deployed at live URL.
* Applcation loads with no errors.
* Application GitHub URL submitted.
* GitHub repository contains application code.

## Application Quality: 11%
* Application console is free of errors.

## Repository Quality: 13%
* Repository has a unique name.
* Repository follows best practices for file structure and naming conventions.
* Repository follows best practices for class/id naming conventions, indentation, high-quality comments, etc.
* Repository contains multiple descriptive commit messages.
* Repository contains a high-quality README file with description, a link to walkthrough video.

## Bonus
Fulfilling the following can add 10 points to your grade.  Note that the highest grade you can achieve is still 100:
* Application allows users to delete notes.