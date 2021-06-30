[title]: # (Introduction)
[tags]: # (mobile)
[priority]: # (1)

# Introduction to the Secret Server Mobile Application

Through the Secret Server Mobile application, users can connect from a mobile device to a Secret Server instance to view, manage, and use secrets stored there. The mobile application interface is similar to the Secret Server interface, which makes it easy for users to navigate to find secrets and secret folders. The mobile application offers useful functionality including multi-factor authentication, biometric authentication, autofill, online and offline caching, and advanced secret workflows, all summarized below.

## Multi-factor Authentication

The mobile application supports the same MFA mechanisms as used by Secret Server:  

* DUO – Push  
* DUO – Phone call
* Pin Code
* TOTP authenticators

## Biometric Authentication

The mobile application supports using biometric authentication in place of usernames and passwords.

* Fingerprint (Android and iOS)
* Facial recognition (iOS only, not all phone/iOS combinations)

The application will auto-reconnect to Secret Server if the connection is temporarily dropped due to network issues.

## Autofill

When a user enables their mobile device's autofill service and then registers Secret Server Mobile with that service, users can launch a web session from a secret on the mobile device and automatically populate username and password login credentials on specified web sites or other mobile applications.

When you select the mobile application or web page and click on the username field you should see a prompt from Secret Server Mobile to use the autofill service. Click this option to open the mobile app and log in if necessary, and the app runs a search of your secrets for:

* Browser web site - to search for any secret that has the same Domain value in the URL
* Other mobile application - to search for any secret that has the same name or URL value as the name of the mobile application that is being filled.

Users can also choose to manually modify the search value and run it again. Once the list of Secret Server Secrets has been returned, you can select which one you want to use and the autofill service will fill those credentials in the related username and password fields.

>**Note**: Currently the autofill service supports only the username and password fields.

## Online Caching

Secure storage handles most of the security:

* on __iOS__, Secure Keychain is used. Keychain items are encrypted using two different AES-256-GCM keys.
* on __Android__, an AES key is obtained from the android key store. This is then used with an AES/GCM/NoPadding cipher to encrypt the value.
* Following login, the online cache displays the user's list of Secrets, without secret details
* The online cache is updated every 5-10 minutes.
* The cache is cleared out on user logout and user switch.
* No credential values are cached, except for the Secret Server login, which is used by Biometrics.

## Offline Caching

An organization can permit its Secret Server Mobile users to save secrets to an offline cache. When a network connection to Secret Server is unavailable, users can access secrets they previously cached offline for a specified Time-To-Live (TTL) period. An organization’s Secret Server administrator controls TTL and access to offline caching globally, for all mobile devices in the organization. If an organization does not allow offline caching, the administrator sets the TTL to zero. To use offline caching, biometric authentication must be enabled.

Offline caching:

* Stores information in a secured encrypted database.
* Stores secrets tagged for offline caching along with their secret details
* Updates automatically by default, unless the auto-update feature is turned off
* The cache is cleared on user logout and user switch.
* Offline mode login is secured by biometric authentication (fingerprint or face ID).

## Secret Workflows

From **Autofill**, **Home**, **Favorites**, **Recents**, and **Shared** screens, Secret workflows provide users with screens, confirmations, notices, prompts, indications, and controls related to:

* checking out and checking in a secret
* submitting, resubmitting, and canceling a request for access to a secret
* submitting a Double Lock password or a Ticket Comment, Reason, or Number to access a secret
* confirmation of submission, approval, denial, or cancellation of an access request
* notification of a duplicate request for access to a Secret
* notification of login failure with the reason for failure
* provision of access to a secret, including details and options, upon approval
* setting a duration and a beginning and end time for accessing a secret, now or at a later date
* visual indication of each secret you have checked out, from both Secret Server Mobile and the Secret Server web interface
* visual indication that a secret is checked out by another user
* entering a Comment and checking out a Secret at the same time
