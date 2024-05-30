# d2l-brightspace-custom-pages
This page is was designed before the widget was created and added to the course homepage.  Using D2L Organization Files, I created an html page, then using external links, I created a link, browsed over to the view all links page and selected this webpage.  I grabbed that link and added this page to the navigation bar and set the permissions to be accessed by the Instructor.  

This page will grab a list, based on time period I set up in the code, of the courses the Instructor is enrolled in as the "Instructor" role.  The instructor has two buttons, enroll ZZStudent or unenroll ZZStudent.  We use ZZStudent as a way for faculty to impersonate and participate in the class like a student to get a full experience.  

## Process
The button, depending on which one you click, will run through the process.  The Enroll Demo Student button will create a new user and attach the course ID number to the end of the user name.  This makes it uniquely set to this course only.  But first, the code before creating the user, will check to see if a user is already enrolled with this unique name.  If so, it will not proceed.  If no user is listed, the code will create the user and enroll that user into the course.  

Mainly the opposite action is done with the Unenroll Demo Student.  The first action is checking to see if the user exists.  Since we are using unique user accounts, it know which student to look for.  If the user is found on the classlist, the code will process and remove the student.  The user account is not deleted, just removed from the course.  This allows the Instructor to add and remove as needed throughout the semester over and over.  This way a new user is not created everytime, just once.  

The reason for this widget and page is to reduce help desk tickets for our Admins, the Instructor can now do it on their own.  

<img width="397" alt="Add ZZ Student" src="https://github.com/justinbamberg/d2l-brightspace-custom-pages/blob/main/add-zzstudent.png">
