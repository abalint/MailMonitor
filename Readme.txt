Author - Andrew Balint
June 3, 2013
v1.0

--------------------------------------

Run MailMonitor.jar to execute the program

To change the email accounts being used, go into the EmailList folder, and edit list.txt
   Put the account name first on a line by its self, with the corresponding password on the following line.

   Currently, the program is only guaranteed to work with gmail.com, aim.com, and other google email accounts, such as houston-offshore.com
   There is a generalized statement for other email address, but they must support both SMTP and IMAP, and their server address must be "smtp.DOMAIN.com" and "imap.DOMAIN.com"

Logs are written to a new file every day, named by date, in the Logs folder. The program does not manage deletion of these logs. 

Emails on the accounts will be deleted after 100 have accumulated. Please be sure not to use your personal account, as it my cause unwanted deletion. 
-------------------------------------

formatting

Output will be given as:
   "success/warning/failure" $-- "sender email address" -> "receiver email address" $-- ms taken $-- time stamp

    warnings and failures will give you additional information as to why they failed, and possibly what you can do to prevent it from happening

$-- is a delimiter in case you want to use the output in different programs. 


------------------------------------

Known bugs

The application will freeze for about 5 seconds between each output. if you try to close the application during this time, it will not work, but will close when it becomes responsive again.
  Work around
      if you really want to kill the application during those 5 seconds, use a task manager to force close application "javaw.exe" 

If you find additional bugs, please report them to abalint@houston-offshore.com
