[title]: # (1.0.1 Release)
[tags]: # (release notes)
[priority]: # (10999)
# 1.0.1 Release Notes

_October 21st, 2020_

## Enhancements

* Onboarding:
  * Added a __Skip__ option to the enable biometric page.
  * Resize toggle switch for using biometric options.
* Autofill service:
  * Improved alert message popup.
  * Updated spinner when loading search screen for autofill.
* Biometrics:
  * Updated default values based on Android/iOS platform for onboarding.
* General User Interface improvements:
  * Updated icons and adjusted alignments.
  * Reduced unnecessary spacing on multiple screens.
  * Modified the location of the __Cancel__ button depending on screen size.
  * Modified size/shape of logged in user avatar on Menu screen.
  * Adjusted screen spacing for keyboard pop-up.
  * Added additional validation on __Edit Folder Name__ field.

## Bugs Fixed

* Fixed an issue where an SSL error is returned upon connecting to Cloud Secret Server instances depending on TLS version.
* Fixed an issue where the confirmation message pop-ups were cut off at the bottom of the dialog on some screens.
* Fixed an issue where the __Apply__ button was enabled on the Password Change screen when no user modifications had been made.
* Fixed an issue with Secrets being listed but inaccessible on the All tab upon users switching accounts.

### Android Specific

* Fixed an Autofill service issue that didn’t consistently open to __Search__ when users were prompted with biometric verification.

### iOS Specific

* Fixed an issue on the Secret Details page for the __Favorites__ icon filling inconsistently when selected.
* Fixed an issue where the wrong message was displayed on an unsuccessful FaceID scan.
