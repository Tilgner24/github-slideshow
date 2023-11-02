# Use case desciptions
| Name:| Login |
|---     |---        |
| Actor: | User |
| Description | The User wants access to the application. |
| Pre-condition | The User needs to be __Registered__. |
| Scenario: |  1. System asks for username and password.  <br>2. User types in his username and password and presses the login button. <br>3. The system checks whether the login data is correct and gives the user access to the application. |
| Result: | The user is logged into the application. |
| Extensions: | 2.1 The user forgot his password and presses the button "Forgot password". <br> 2.2 The system asks for his e-mail. <br> 2.3 The user types in his e-mail. <br> 2.4 System sends his password to the typed in e-mail. <br> Continue with step 2.|
| Exceptions: | 3.1 User typed in a wrong username or password.  <br>3.2 System shows a message "wrong username or password please try again".<br> Continue with step 2.|
----------------------------------------------

| Name:| Look up challenge |
|---     |---        |
| Actor: | User |
| Description | The User wants to search for a specific challenge. |
| Pre-condition | There has to be existing challenges in the database.|
| Scenario: |  1. System shows a searchbar. <br> 2. User types in the name of the challenge. <br>3. The system shows all the challenges that are named like the search term.|
| Result: | The User recieves a list of challenges that named like the search term. |
| Extensions: | 2.1 System cant find any challenge that are named like the search term and shows a little text "Can't find any challenges named like that".|
| Exceptions: | none |
----------------------------------------------
