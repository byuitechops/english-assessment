# Mass Feedback Setup

### Getting Started
1. Create your copy of the "Mass Feedback" sheet and "Today's Response" forms
    * [Form Template](https://docs.google.com/forms/d/1--ST9Rpz3HAj8V7tBMv5vr-nmlkkNVe0MjA8vy0buDg/edit)
    * [Sheet Template](https://docs.google.com/spreadsheets/d/1lP4ui2fQzNlHhJiet2fyjQt5eVqDtlPYfvtghEA170g/edit#gid=271771189)

2. Ensure that the form and sheet are linked by testing the form
    * *To learn how to link Google Forms to Sheets use [this support document](https://support.google.com/docs/answer/2917686?hl=en)*

3. In cell A2 of the "question links" page, add the direct link to your form

4. Set up your questions as deisred
	* The formula to build the url in the "brightspace checklist link" is:
    
    > ```=IF(A4 = "","",REGEXREPLACE(REGEXREPLACE($A$2,"(\$DAY\$)",(A4)), "(\$QUESTION\$)", B4))```
    
    note: *"4" is the first usable row in the sheet, each row's formula requires the number of the current row.*

5. You can test your question links by copying and using one of the URLs generated by your sheet.
    * *If the "Question" field of your form matches the question you created for that row, you know it is working*

6. Add the links to the form into your course

### Providing Feedback

1. Click the "Student Data" menu above your toolbar and select "Pull Student Data" to ensure that your student responses are up to date.

2. Select "Student Response Viewer" from the same menu to open the Response Viewer sidebar.

3. Use the "Days", "Courses", or "Students" fields to filter your search then click "View Responses"
    * At this point the tool builds your "view Response" sheet and redirects your focus to it.
    
4. Set up your signature in the "signature" field then fill out your "Canned Responses" with the general feedback you would like to give your students

5. Provide Feedback
    * To give a student personalized feedback, add your comments to the "Feedback" column of the "View Response" sheet
    * To give a student a canned response, simply put the number of the response in the "Feedback Rating" column
    
    note: *Students may be given both personal and canned feedback. When you "Save Responses" the canned response is always appended to whatever feedback you have already provided in the Feedback column. *
    
6. Save your feedback by pressing "Save Responses" in the "Student Response Viewer" window, this will append the text of your canned response to the student's "Feedback" column

7. When you have finished preparing and saving responses (ensuring that the "Feedback" column is filled out) you may send the responses by clicking "Student Data" again above the toolbar and then "Send Feedback".
