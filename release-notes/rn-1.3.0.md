[title]: # (1.3.0 Release)
[tags]: # (release notes)
[priority]: # (10998)
# 1.3.0 Release Notes

_November 24th 2020_

## Features

* [SAML Login Support](../onboarding/app.md) (Web Login)  
  * UI Option to use local login or Web Login (SAML)  
  * On the login screen user has the option to [Switch Login](../using/switch-login.md) or [Refresh Web Login](../using/refresh-web-login.md). 
  * When logging in via the Web Login (SAML) user does not have to manually click on “generate token” this is done for the user in the background (some users may see the page flash).

### User Interface Improvements

* When Clicking on search (magnifying glass) and other options, the keyboard won't be active anymore when no text input is required.
* Moved the Home “+” button to the bottom of the screen.
* __Next__ will only be enabled when all required fields are populated.
* __Save__ will only be enabled when all required fields, for example the folder name when creating a folder, are populated.

## Bugs Fixed

* Removed the invalid __Help__ link, when using Auto-fill to fill passwords on an external application.
* Fixed an onboarding issue related to the FaceID/Fingerprint screen when biometrics have not been enabled on the device. Users are presented with a message recommending they enable biometrics for extra security.
* Fixed a defect where Autofill was not working after switching the logged in user to another user.
