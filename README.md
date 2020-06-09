Android
ToDo List by Gabriel Stanev
F№: 1809011299

Description:

I. Design
1) in activity_main.xml we add a <ListView> with an id "listView"
2) then create floating action button for adding new Notes int the ListView
3) we create onClick to trigger "onClick" method which will be created later..
4) creating a new layout for the input of the user with EditText for input with a hint and gravity to display the input
 from the top left corner and another event listener, triggering
 "saveButtonClicked" method

II. Code
- the onClick Method created an Intent that sets the class of that onclick to "EditFieldActivity", then starts activity
 for result.
- the the editFieldActivity class we get the message via the id of the EditText field and if there's no input it does
 nothing anf it there is we make an intent to set that value with the result key
- also i have created a class only for Constants for those PutExtra methods
- now the Edit class (EditMessageActivity) has a saveButtonClicked method
 that finds the clicked message from the list and via setResult with a second constant result code from the helper class
"Intent_Constants" that has qnique keys for "edit" and "add" functions
- finally (and most shamefull), i did not use Firebase or anything like this.
- I remembered for the PrintWriter and the Scanner classes and decided to catch the back button event and
just println the contents of the arraylist in a txt file line by line(which obviously has its flaws),
 and when the app is reopened, just scan the txt file line by line.

P.S. I hope it is not a problem that the description is in english.
