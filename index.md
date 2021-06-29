[title]: # (Introduction)
[tags]: # (mobile)
[priority]: # (1)

# Introduction to the Secret Server Mobile Application

Through the Secret Server Mobile application, users can authenticate to a Secret Server instance to access and use secrets from a mobile device. The mobile application displays secrets in an interface similar to the Secret Server interface, and users can navigate in the mobile application to view secrets and secret folders.

By registering Secret Server Mobile with a mobile device's autofill service, users can launch a web session from a secret on the mobile device and automatically populate login credentials on specified web sites. With bioauthentication enabled, users can save secrets in an offline cache for a specified period so they can access them when they cannot access their Secret Server instance.

## Multi-factor Authentication

The mobile application supports the same MFA mechanisms as used by Secret Server:  

* DUO – Push  
* DUO – Phone call
* Pin Code
* TOTP authenticators

## Offline Caching

An organization can permit its Secret Server Mobile users to save secrets to an offline cache. When a network connection to Secret Server is unavailable, users can access secrets cached offline for a specified Time-To-Live (TTL) period. TTL and access to offline caching are controlled by an organization’s Secret Server administrator globally, for all mobile devices in the organization. If an organization does not allow offline caching, the administrator sets the TTL to zero. Accessing secrets saved to an offline cache requires using biometric face or fingerprint recognition.

## Biometric Authentication

The mobile application supports using biometric authentication in place of usernames and passwords.

* Fingerprint (Android and iOS)
* Facial recognition (iOS only, not all phone/iOS combinations)

The application will auto-reconnect to Secret Server if the connection is temporarily dropped due to network issues.

## Mobile Data Caching

The following security-based information should be considered:

* Secure storage handles most of the security:
  * on __iOS__, Secure Keychain is used. Keychain items are encrypted using two different AES-256-GCM keys.
  * on __Android__, an AES key is obtained from the android key store. This is then used with an AES/GCM/NoPadding cipher to encrypt the value.
* Online cache storage:
  * List of Secrets, without Secret details following the login.
  * The cache is __cleared__ out, on __user logout__ and __user switch__.
  * Cache is updated every 5-10 minutes.
  * No credential values are cached, except for the Secret Server login, which is used by Biometrics.
* Offline cache storage:
  * Stored in a secured encrypted database.
  * Stores secrets and secret details when tagged for offline caching
  * Cache is automatically updated (default) unless the auto-update feature is turned off.
  * The cache is cleared on user logout and/or user switch.
  * Offline mode login is secured by biometric authentication (fingerprint or face ID).