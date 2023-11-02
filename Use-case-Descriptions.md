# Use case desciptions
| Name:| Login |
|---     |---        |
| Actor: | User |
| Description | The User gets access to the application |
| Pre-condition | The User needs to be __Registered__. |
| Scenario: |  1. System asks for username and password.  <br>2. User types in his username and password and presses the login button. <br>3. The system checks whether the login data is correct and gives the user access to the application. |
| Result: | The user is logged into the application |
| Extensions: | 2.1 The user forgot his password and presses the button "Forgot password" <br> 2.2 The system asks for his e-mail <br> 2.3 The user types in his e-mail <br> 2.4 System sends his password to the typed in e-mail. <br> Coninue with 2. again|
| Exceptions: | 2. User typed in a wrong username or password  <br>2.1 System shows a message "wrong username or password please try again"|
----------------------------------------------
