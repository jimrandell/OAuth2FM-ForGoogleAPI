[![OAuth2FM-ForGoogleAPI](https://raw.githubusercontent.com/jimrandell/OAuth2FM-ForGoogleAPI/master/OAuth2FM_Logo1.png)](http://jimrandell.com)

## A Simple Dashboard And A Single Script Provide FileMaker Developers With A Powerful Tool To Handle The Heavy Lifting in Google’s OAuth2!
…No Plugins, No Custom Functions, Just FileMaker

![](https://raw.githubusercontent.com/jimrandell/jimrandell.github.io/master/OAuth2FMscreenshot.png)

*	Create and Manage multiple Google OAuth2 Account Profiles, each with multiple variations of privileges for that Account

*	Present your users with Google’s Login Page, followed by Google’s Page prompting a user to ‘Allow Access To Your Google Account Data’

*	Ready to use as a separate file with your solution – Simply Call 1 Script

*	Incorporate into your own solution – using 2 Layouts, 1 Table, and 1 Script (with 2 subscripts)

*	Optional Value Lists (and one table for Value List reference) are not required, but streamline Profile creation on the dashboard

---

#### Lots Of Help:
*	The HELP Buttons provide step by step instructions with annotated screen shots, so that creating a Google Developers Account, and obtaining your authentication Tokens, is as easy as Pi to the 2nd power!


---

#### CODING PHILOSOPHY:
The Scripts and Calculations in this solution, as with everything I do in FileMaker, are written for the next developer.  
With that in mind:

- **Calculations** are written in the vernacular taught to my by my 5th grade algebra teacher: **SHOW YOUR WORK**  
To that end, I make extensive use of the LET Statement, to show you, the reader, the logical progression of the values as they are manipulated and evolve.
	- 	…sometimes at the expense of brevity, but always to the benefit of clarity and safety, as well as for the consideration of those without access the FileMakerPro Advanced.
- **Global Variables** and **Internal SQL Calls** are strictly avoided (and not used at all in this Module)
They are powerful tools, but they add complications to Interconnecting Modules and hinder portability.

- **Scripted Finds** are written out long (Enter Find Mode, Set Field, Perform Find)  
(With few exceptions) this makes scripts easier to read and comprehend by other developers

- **Scripts Are Well Documented**, forming an overall, step by step narrative.  
Liberal use of white space is made, separating the code into ‘easily digestible’ chunks.


---


#### TODO:
A second set of scripts using Custom Functions, and accepting all the required values passed as Parameters,
has been pushed back for the next release, pending feedback received by this initial release.

