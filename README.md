# TableauVoiceWebApplication
A web app that uses the webspeech and Tableau APIs to allow users to manipulate tableau worksheets with their voice, mouse, or text.


# Requirements for Use
The application requires a system that allows you to open it on a suited web browser.
For best results, run the application in Google Chrome or Mozilla Firefox but it should
work in any modern web browser. To properly interact with the software, ensure that
your system has a working microphone that the browser can recognize and access.



# Application Flow
The login page is mostly just for show. It mostly demonstrates my use of local storage to 
give the web app a more personal touch as it remembers your name as well as your last 3 
Tableau worksheets that you worked on while using the app

The application provided requires that you supply a tableau worksheet URL which it then
allows you to manipulate in our environment by just using your voice. Once the
worksheet is open you are able to click and manipulate it as you normally would with a
mouse but you are also able to execute the same commands by using your voice and
following the given instructions located in this manual.


# List of legal commands
 
# Command                                     Response
Exit, Hide, or Close                          Hides the Tableau window

Reload                                        Reloads the page

A specific filter name with ‘add’ a
nd synonym of add(example:'add', 'ad',
'ed', 'at', 'plus', 'put in', 'include')      Add a specific filter into current field

A specific filter name with synonym of 
remove(example: 'remove', 'reduce', 'delete') Remove a specific filter from the current field

A specific filter name without 'add', 'ad',
'ed', 'at', 'plus', 'put in', 'include', 
'remove', 'reduce', 'delete'                  Default action when detect a filter name, it will replace all the filters in the current                                                 field into this specific filter

A specific field name with synonym of reset 
(example: 'reset','all', 'everything',
'clear', 'reload', 'refresh')                Reset this field by adding all the filters into it


A specific field and filter name with
synonym of add (example:'add', 'ad', 'ed',
'at', 'plus', 'put in', 'include')           Add a specific field which belongs to this specific field into this field (example: For a                                                filter based on ‘States’ ”add Texas” unhides Texas)


A specific field and filter name with
synonym of remove (example: 'remove', 
'reduce', 'delete')                          remove a specific filter which belongs to this specific field from this field (example: For                                              a filter based on ‘States’ ”remove Texas” hides Texas)


A specific field and filter name without
'add', 'ad', 'ed', 'at', 'plus', 'put in',
'include', 'remove', 'reduce', 'delete'      Default action when detect both a field and filter name, it will replace all the filters in                                              this specific field into this specific filter


Any command with a tab name                  Switch to the tab which has the name appeared inside the command (example: The command                                                  “Economy” switches to the tab Economy if exists)


“help”                                       Program will speak the names of supported field names back to you.
“ignore”                                     Stop listening
