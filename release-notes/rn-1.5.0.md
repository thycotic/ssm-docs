[title]: # (1.5.0 Release)
[tags]: # (release notes)
[priority]: # (10996)
# 1.5.0 Release Notes

_March 16, 2021_

## Features

Secret Server Mobile 1.5.0 is a hotfix release to support devices running the iOS update 14.4.1.
Otherwise the functionality and features included in this release are identical to those provided by the 1.4.0 release, which provides users with the following enhanced capabilities, including workflows for the following actions:

* check in and check out Secrets
* provide a **Double Lock** password to access a Secret
* provide a **Comment** required to access a Secret
* provide a ticket Number required to access a Secret
* provide a Reason required to access a Secret
* receive a notification when you have requested access to a Secret twice in a row
* see a visual indication of each Secret you have checked out from both Secret Server Mobile and the Secret Server web interface 
* see a visual indication when you request access to a Secret that is already checked out by another user 
* set the beginning and end dates and times for checking out a Secret
* cancel requests for access to Secrets at any stage of the request process

## User Interface Improvements

* Changed the password font to clearly distinguish between adjoining letters lowercase “l” (L) and uppercase “I” (I).

## Bugs Fixed

* If your attempt to log into Secret Server fails, you now receive a message with the reason for the failure, such as incorrect username/password, failed 2FA/MFA input, no internet connectivity, incorrect Secret Server URL, 500 error from Secret Server, or no permissions/access to use the REST APIs. 
* When you request access to the same Secret twice in a row, Secret Server Mobile now notifies you that you have already requested access to that Secret.  
* In the **Title bar**, Secret names are no longer truncated when there is sufficient room to display them. 
* When Secret Server Mobile cannot use **FaceID**, it now displays an appropriate notification. 
* After a screen is minimized or maximized, the screen now retains all the information you already entered.  
* After a screen is minimized or maximized, the keyboard is no longer displayed on the **Fingerprint ID** screen 
* When a user cancels out of the **Fingerprint ID login** or the attempt has failed, the notification screen that appears no longer displays a keyboard. 
* When a user cancels out of the **Fingerprint ID Login** and opens the **Password Login**, Secret Server Mobile no longer crashes. 
* After Secret Server Mobile displays a **Face Not Recognized** message and the user taps **Enter Password**, the keyboard is now displayed. 
* When API errors occur, Secret Server Mobile now displays relevant notifications. 
* After a user deletes a Secret, Secret Server Mobile now displays a notification that the deletion was successful. 
* When a site certificate is not valid, Secret Server Mobile now displays an appropriate message instead of **URL is not valid**. 
* The **Home** screen now opens when expected, whereas in some cases the **Secrets** list screen appeared instead (SAML/Web Login) 
* When you enter a correct Double Lock password for a Secret or Secrets, the Double Lock password is cached so you do not need to manually re-enter it for the remainder of the session. If the session expires, you will need to re-enter the Double Lock password. 
 
## Known Issues

* In some situations, when a user on an iOS device attempts to connect to a Secret Server Cloud using SAML (Web Login), the authentication token does not seem to successfully get back to the mobile app, resulting in a gray screen with a spinner icon.
* On iOS devices, a Toaster message at the top of the Secret Server Mobile **Home** screen overlaps the phone’s system indicators such as the time and carrier.
* Users attempting to connect to an on-premises Secret Server configured with a Self-Signed/Internal certificate receive the message, **Unable to connect due to a self-signed or untrusted certificate**.
* When a user is creating a Secret using the template **Generic Discovery Credentials** and taps to enter a **Private Key Passphrase**, the input field should display **Enter** instead of **Current Password**, and the button label should read, **Generate** instead of **Generate Password**. It will generate a strong password.
* When Secret Server Mobile is auto-filling a password from a Secret that requires edit privileges to view it, the password field is filled with, **Not Valid for Display** instead of the actual password.
* Secret Server Mobile does not currently support deployment via MDM solutions (VMware workspace/AirWatch etc.)
* When a user attempting to access a Secret enters an incorrect alphanumeric value in the **Ticket Number** field, the error message, **Failed to send access request** appears.
* Secrets checked out by the current user via Autofill are not marked as **Checked Out** on the main screen. Likewise, Secrets marked as **Checked Out** on the main screen are not marked **Checked out** when using Autofill.


