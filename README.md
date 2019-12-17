# RebateForm_WindowsFormApp
Data entry app designed using Windows Form .NET Framework which uses a .txt file for reading/writing and storing customer data

 Specifications are as follows:
1.	The file (and therefore the screen) will contain the following fields: 
a.	First name (20)
b.	Middle initial (1)	(may be blank; entry not required)
c.	Last name (20)
d.	Address line 1 (35)
e.	Address line 2 (35) 	(may be blank; entry not required)
f.	City (25)
g.	State (2)
h.	Zip code (9)
i.	Gender (1)  (M or F)
j.	Phone number (21)
k.	E-mail address (60)
l.	Proof of purchase attached (Yes/No)
m.	Date received (default to today but changeable)
2.	The following fields will be in the file but are added by your program, not the user, and are not visible to the user.  Add them only when adding new records, and do not change them if a user modifies a record.
a.	The time at which the user first entered a character into the first field, accurate to the second.
b.	The time at which the user pressed the Save button.
c.	The number of times the user pressed the backspace key during data entry.  This can be obtained by processing a keystroke event, and will be explained.
3.	Your program must provide three functions: 
a.	Add a new record to the end of the file.
b.	Modify an existing record and write it back to the file.  This means that you can modify all fields of the record, including the name, but not the three invisible fields.
c.	Delete a record from the file.
4.	Your program must not be able to add a record that contains the same first name, last name, and phone number as a record already in the file.  You must not be able to modify an existing record such that the modification violates this rule, either.  In general, your program must not be able to enter bad data into the file.  That is, dates must be checked for validity, for example.  On the other hand, there is no way to check a person’s name for validity.
5.	Data file handling:  Below are the requirements (not suggestions) for the data file.
a.	Since this is not a database class, you will use a flat text file with one record per line.  Fields are separated by tabs.
b.	 If the file does not exist, your program must create it.
c.	The name of the file is CS6326Asg2.txt.  You will lose five (5) points for using any other file name.  Do not have any information other than the file name.  For example, using a file with a name like c:\users\jxc064000\CS6326\CS6326Asg2.txt is not acceptable and will cost you 20 points.
d.	The fields must be written in the order given above, with two additional fields given below that are not entered by the user.
e.	When the program starts, read the entire file into memory.  When a user saves data, write the entire file. 
6.	“But C# has database functionality.  Can we use that?” No.
7.	You may not read everything into a datagrid or something like it and treat it as a spreadsheet.  You must have separate fields for the various data elements.  (One issue with using a datagrid is that the user will have to side-scroll, which is poor design.  A second issue is that in a real system there could be thousands of records, but a real system would have functionality I’m not requiring and take too long to program.)
8.	You should show the full name and phone number only (not every field) in a multi-column scrollable list. Clicking on a list item should put all of its data elements into the fields for modification.  That is, if a name is selected from the list, the clerk should be able to save the changes or discard them.
9.	All three functions must be done from the same main screen.  There should be no menu and no multiple screens.
