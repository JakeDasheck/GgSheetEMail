# GoogleSheetEMailSender 
## Script to sending automatically emails for Google Sheet users.

* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)

## General info
This project is a Google Sheets script which automatically sends the email messages to users which were assigned to dates in table.
The script compares the dates and send the email message to the person which was assigned to the date.
	
## Technologies
Project is created with:
* App Script
* JavaScript
	
## Setup
To use this script you have to:


1. Make a new Google Sheet file and make two sheets in it.
2. You need to name the sheets as follows: "Calendar" and "emailAddresses" (without quotation marks).
3. The "Calendar" sheet has to look like screenshot below:

a. In the A ("Day") column you have to write a date when scritp should send the e-mail.
b. OPTIONAL In the B ("Day of the week") you can write a day of the week, when the script should send the e-mail.
c. In the C ("Name Surname") column you have to write name and surname of addressee.
![Calendar sheet](Images/Calendar.png)

4. The "emailAdresses" sheet has to look like screenshot below:
a. In the A ("Name Surname") column you have to write name and surname of addressee.
b. In the B ("Email Address) column you have to write a e-mail adresses for each addressee. 
![emailAdresses sheet](Images/emailAdresses.png)

5. Than, you have open the script editor from: Tools -> Script Editor and make a new project.
6. Next, go to my GgSheetEMail repository, copy entire script from it (EmailSender file) and paste it into the script editor.
7. Than, save it and name your script.
8. Now you have to make a triggers. Go to Current project's triggers from Edit menu and make Add Trigger.
9. There you have to set options as follow:
a. "Choose which function to run to" set to "CheckColumnDate"
b. "Which runs at deployment" set to "Head"
c. "Select event source" set to Time-driven
d. "Select type of time based trigger" set to "Day timer"
e. "Select time of day" set the time when the script should send the e-mail.
and save it.

10. Than you have to give all permisions for script to run on your Google account. 

That's all. :)


