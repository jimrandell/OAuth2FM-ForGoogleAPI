# OAuth2FM-ForGoogleAPI
Make calls to GoogleAPI from FileMaker, and let this module handle the Tokens and Authentication.



#A Simple Dashboard And A Single Script To Call, Provides FileMaker Developers With A Powerful Tool!
*	Create and Manage multiple Google Account Profiles, each with multiple variations of privileges for that Account

*	Present your users with the Googles Login Page, followed by the Google page which prompts users to 'allow this app access to your Google Account Data'

*	Ready to use as a separate file with your solution - Simply Call 1 Script

*	Incorporate into your own solution** - using 2 Layouts, 1 Table, and 1 Script (with 2 subscripts)  
Optional Value Lists (and one table for Value List reference) are not required, but streamlineProfile creation on the dashboard


'

'

----
'


##Use Case 1
**Use this individual File as part of your overall solution, calling the OAuth_Processor Script like an API call**

1.	 Open this file, and create and name an Authentication Profile on the Dashboard.
	*	comprehensive help is provided on the Layout, explaining exactly how to populate the fields

2.	 Call the OAuth_Processor Script from inside your solution, the script returns the valid Token(s) required to make a Google API Call
	*	Optionaly, include the Profile Name as the Script Parameter
	*	Passing no Parameter will use the Profile in the Active record from the Profile Table 
	*	additional documentation is found in the Comments of the OAuth_Processor Script (and on-screen help)

3.	Open the OAuth_Example_APIcall Script in the Examples and Tests Folder
	*	Here you will find an example use case
	*	Also, open and read the comments in the Script: OAuth_Processor


'

'


##Use Case 2
**Import the components of this file into your solution.**  
(do not re-name anything until you have fully tested it in your own solution)

1.	 Import the OAuthProfiles Table (or copy it if you have FMP Advanced)  
	*	Open your FileMaker file, Select Manage>Databases from the File Menu
	*	Select the 'Tables' Tab, click the 'Import...' button, and select the OAuthProfiles Table from this file.

2.	 Create two Layouts for the OAuthProfiles Table Occurence, name them "OAuthProfiles_Dashboard" and "OAuthProfiles_WVpopup"
	*	Optionally, incorporate the Value Lists Table
		*	Import the OAuthScopes Table the same you you imported the OAuthProfiles
		*	Recreate the Value Lists in your own file, exactly as they exist in this one

3.	 Import the OAuth2FM Scripts Folder into your Modules Scripts Folder: (or copy it if you have FMP Advanced)
	*	Open your FileMaker file, Select Manage>Scripts from the File Menu 
	*	Click the 'Import...' button, and select the OAuth2FM Scripts Folder
	*	Move the OAuth2FM Scripts Folder into your Modules Scripts Folder
		*	If you dont have a Modules Scripts Folder, Create one (a Scripts Folder Called "Modules")


4.	 Paste the Objects from the 2 Layouts
	*	Go to the OAuthProfiles_Dashboard Layout in this file, Enter Layout Mode, Select All,and Copy
		*	Go to the OAuthProfiles_Dashboard Layout in YOUR file, Enter Layout Mode, Select All, Delete, then Paste
		*	Do the same for the OAuthProfiles_WVpopup


5.	 Follow steps 1, 2, and 3 as described in Use Case 1
	*	Here you will find an example use case
	*	Also, open and read the comments in the Script: OAuth_Processor

'

'

----
'

##CODING PHILOSOPHY:
The 'Non-User Facing' aspects of this solution, as with everything I do in FileMaker, is written in consideration of the next developer  
With that in mind:

- **Calculations** are written in the vernacular taught to my by my 5th grade algebra teacher: **SHOW YOUR WORK**  
To that end, I make extensive use of the LET Statement, to show the reader (you) my logical progression as I manipulate the values
	- 	sometimes at the expense of brevity, but always to the benefit of clarity and safety, as well as for the consideration of those without access the FileMakerPro Advanced
- **Global Variables** are strictly avoided (and not used at all in this Module)
they are a powerful tool that work best when they are used as little as possible

- **Scripted Finds** are written out long (Enter Find Mode, Set Field, Perform Find)  
(With few exceptions) this makes scripts easier to read and comprehend by other developers

- **Internal SQL** calls are not used  
and, in my opinion, should only be used by the Lead, or Primary Developer (as with Global Variables)


'

'

----
'

##TODO:
A second set of scripts using Custom Functions, and accepting all the required values passed as Parameters,
has been pushed back for the next release, pending feedback received by this initial release.

