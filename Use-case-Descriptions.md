# Use case desciptions
| Name:| Login |
|---     |---        |
| Actor: | User |
| Description | The User wants access to the application. |
| Pre-condition | The User needs to be <u>Registered</u>. |
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
| Scenario: |  1. System shows a searchbar. <br> 2. User types in the name of the challenge. <br>3. The system shows all the public challenges that are named like the search term.|
| Result: | The User recieves a list of challenges that named like the search term. |
| Extensions: | 2.1 System cant find any challenge that are named like the search term and shows a little text "Can't find any challenges named like that".|
| Exceptions: | none |
----------------------------------------------

| Name:| Join the challenge |
|---     |---        |
| Actor: | User |
| Description | The User want to be part of a challenge and joins it. |
| Pre-condition | The challenge has to be existing.|
| Scenario: |  1. The System shows a list of challenges. <br> 2. The user presses on a challenge he wants to join. <br> 3. The system shows all the details about the challenge and a button that says "Join!." <br> 4. The User presses on "Join!". <br> 5. System adds the user to the challenge.|
| Result: | The User jointed the challenge and is now part of it. |
| Extensions: | 1. The user recieves an invitation for a private challenge and presses on it. <br> Continue with step 3.|
| Exceptions: | none |
----------------------------------------------

| Name:| Decline the challenge |
|---     |---        |
| Actor: | User |
| Description | The User don't want to join the challenge he got invited to |
| Pre-condition | The challenge has to be <u>shared</u> to the user.|
| Scenario: |  1. The system shows all the details about the challenge and a button that says "decline."<br> 2. The user presses on "decline". <br> 3.The system informs the invitor that the invited declined the challenge.|
| Result: | The User declinded the challenge and the invitor is informed. |
| Extensions: | none |
| Exceptions: | none |
----------------------------------------------

| Name:| Choose moderators |
|---     |---        |
| Actor: | User |
| Description | The user selects one or more users within a challenge and gives them moderator rights. |
| Pre-condition | The challenge needs participants. The User needs to be the owner of the challenge |
| Scenario: |  1. The System shows a list of all participants. <br> 2. The user selects one or more user. <br> The System asks to give them the rights of a moderator via a button that says "Give moderator rights" <br> 3. The user presses on "give moderator rights" <br> 4. System gives the selected users moderator rights. <|
| Result: | The selected user have moderators rights now. |
| Extensions: | none |
| Exceptions: | none |
----------------------------------------------

| Name:| Edit moderators |
|---     |---        |
| Actor: | User |
| Description | The user selects one or more users with moderator rights within a challenge and takes the moderator rights away. |
| Pre-condition | The owner had to __Choose moderators__. |
| Scenario: |  1. The System shows a list of all participants. <br> 2. The user selects one user with moderator rights. <br> The System asks to take the rights of a moderator away via a button that says "Remove moderator rights" <br> 3. The user presses on "Remove moderator rights" <br> 4. System takes away moderator rights for the selected users. <|
| Result: | The selected user lose their moderators rights |
| Extensions: | none |
| Exceptions: | none |
----------------------------------------------

