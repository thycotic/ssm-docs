[title]: # (Configuring the Mobile Application)
[tags]: # (mobile,configuring,configuration)
[priority]: # (400)

# Configuring the Mobile Application

## Enabling Web (SAML) Login

SAML support allows users to login via Web Login.

To use the Web Login option

1. Navigate to your Secret Server Mobile apps login screen.

1. Enable the __Web Login__ switch.

   ![switch](images/web-login-switch.png "Setting the Web Login switch to on")
1. Click __Continue__. You will see a quick page flash when the app reaches out to the server for the token generation.

   Your Login page now looks like this:

   ![login](images/username-pwd.png "Web Login page")

## Enabling Biometric Authentication

Thycotic recommends using biometric authentication: either facial recognition (iOS only) or fingerprint ID (Android and iOS) in place of username and password credentials. You must enable biometric authentication to use offline caching features.

1. Navigate to the **Settings** page and select either fingerprint identification or facial recognition.

   ![enable autofill](images/init-5.png "Settings page: Use AutoFill")

1. Click __OK__ at the trust prompt and follow the directions to enter your fingerprint.

## Enabling Autofill

1. On the **Settings** page you can choose automation settings including **Use AutoFill** for usernames and passwords.

   ![enable autofill](images/init-5.png "Settings page: Use AutoFill")

1. On the **Use Autofill** page, follow the directions and click **Go To Device Settings**.

   ![autofill](images/init-4.png "Enable autofill functionality prompt on initial login")
