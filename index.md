[title]: # (Introduction)
[tags]: # (mobile)
[priority]: # (1)

# Introduction to the Secret Server Mobile Application

The Secret Server Mobile application allows business users to access Secrets including login credentials on Secret Server from a mobile device. Users can save secrets in an offline cache for a specified period so they can access them when they cannot access their Secret Server instance.

## Multi-factor Authentication

The application supports the same MFA mechanisms as used by Secret Server:  

* DUO – Push  
* DUO – Phone call
* Pin Code
* TOTP authenticators

## Biometric Authentication

If available via device, the application supports biometric authentication instead of a Secret Server password:

* Fingerprint (Android and iOS)
* Facial recognition (iOS only)

The application will auto-reconnect to Secret Server if the connection is temporarily dropped due to network issues.
