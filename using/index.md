[title]: # (Using the App)
[tags]: # (mobile)
[priority]: # (3)
# Using the Application

The application will display the Secrets in a UI similar to the Basic dashboard in Secret Server. Clicking on
a Secret will expand it and show the Secret information. You will be able to edit and open the Secret in
browser. Clicking Edit allows you start editing the contents of the Secret.

The mobile app can be used to authenticate to a Secret Server instance (on-prem or cloud) and access secrets.

## Supported MFA

The application supports the same MFA mechanisms as used by Secret Server:  

* DUO – Push  
* DUO – Phone call
* Pin Code
* TOTP authenticators
* FIDO (NFC)

If available via device, the application supports biometric authentication instead of password or other types of MFA:

* Fingerprint (Android and iOS)
* Facial recognition (iOS only)

The application will auto-reconnect to Secret Server if the connection is temporarily dropped due to network issues and support for Secret Server login refresh token.

## Functional Scope

Ability to run the following actions for both Secrets and Folders:

* View, add, edit, delete
* Search based on:
  * Name
  * Template
* Favorite
  * List from SS
  * Can add Secrets to list from Star icon in mobile app
* Recent
  * List of most recently accessed Secrets
  * Limit list to last 15

Users access and use their secrets via mobile device, using the built-in password management features. When Users are logged in with their own account, users can navigate the Sectret Server folder structure to access any of their Secrets.
The applications allows users to automatically fill credentials from Secrets into other mobile apps or Web browser sites on the mobile device. For this to work correctly, the application needs to be registered with the device's autofill service.

The application allows users to launch a web session from a Secret on the mobile device and have the credentials auto-populate in the mobile devices default browser.
