[title]: # (1.4.0 Release)
[tags]: # (release notes)
[priority]: # (10997)
# 1.4.0 Release Notes


_March 24, 2021_

## Features

Secret Server Mobile 1.4 provides users with the following enhanced capabilities, include full-featured workflows for actions directly from the Autofill screen: 
* provide a Double Lock password to access a Secret
* provide a Comment required to access a Secret
* provide a ticket Number required to access a Secret
* provide a Reason required to access a Secret.
* receive a notification when you have requested access to a Secret twice in a row
* receive a notification with the reason for a failed attempt to log into Secret Server 
* see a visual indication of each Secret you have checked out from both Secret Server Mobile and the desktop Secret Server application 
* see a visual indication when you request access to a Secret that is already checked out by another user 
* set the beginning and end dates and times for accessing a Secret
* cancel requests for access to Secrets at any stage of the request process

## Bugs Fixed

* In the title bar, Secret names are no longer truncated when there is sufficient room to display them.
* When Secret Server Mobile cannot use FaceID, it now displays a relevant notification.
* After a screen is minimized or maximized, generated passwords now remain displayed. 
* After a screen is minimized or maximized, the keyboard is no longer displayed on the Fingerprint ID screen.
* When a user cancels out of the Fingerprint ID Login or the attempt has failed, the notification screen that appears no longer displays a keyboard.
* When a user cancels out of the Fingerprint ID Login and opens the Password Login, Secret Server Mobile no longer crashes. 
* After Secret Server Mobile displays a Face Not Recognized message and the user taps Enter Password, the keyboard is now displayed. 
* When API errors occur, Secret Server Mobile now displays relevant notifications.
* New text options for iOS now clearly distinguish between a lowercase letter ‘L’ (l) and an uppercase letter “i” (I). 
* After a user deletes a Secret, Secret Server Mobile now displays a notification that the deletion was successful.
* When a site certificate is not valid, Secret Server Mobile now displays an appropriate message instead of *URL is not valid.* The Home screen now opens when expected, whereas in some cases the Secret list screen appeared instead. 
* When you enter a correct Double Lock password for a Secret or Secrets, the Double Lock password is cached so you don’t need to manually re-enter it for the remainder of the session.   
