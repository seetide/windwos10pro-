# windwos10pro-
set up new local user

Heather Hamilton #17Replied on August 2, 2018
I have just been sweating through this issue myself.  I think I have found a solution:

Click the start button and type "Edit Group Policy" and select the control panel option of that name.
In the left-hand pane, navigate to "Computer Configuration\Administrative Templates\System\Logon" .
Double click on "Enumerate local users on domain-joined computers" in the right hand pane.
Turn it on via the "Enabled" radio button.
Click "OK".
Check that "Hide entry points for Fast User Switching" is NOT enabled (it can be either enabled or not configured).
Close the Local Group Policy Editor.
Check that users are visible in the switch account menu and on the login page.
Hope this saves someone else the hours I have spent finding that solution.
