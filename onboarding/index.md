[title]: # (Onboarding)
[tags]: # (mobile)
[priority]: # (2)
# System Requirements

The following Operating Systems are supported:

* iOS 12 and up
* Android 8 and up

Minimum hardware requirements mobile devices running the above OS version and not being older than four years.

## Compatibility

The Secret Server Mobile Application works with Secret Server on-premises and cloud instances starting with Version 10.8 and up. To utilize Secret Server's __onboarding feature__, Secret Server 10.9 is a minimum requirement.

The mobile application integrates via Secret Server's RESTApi.

## Mobile Data Caching

The following security based information should be considered:

* Secure storage handles most of the security:
  * on __iOS__, Secure Keychain is used. Keychain items are encrypted using two different AES-256-GCM keys.
  * on __Android__, an AES key is obtained from the android key store. This is then used with an AES/GCM/NoPadding cipher to encrypt the value.
* Cache storage:
  * List of Secrets, without Secret details following the login.
  * The cache is __cleared__ out, on __user logout__ and __user switch__.
  * Cache is updated every 5-10 minutes.
  * No credential values are cached, except for the Secret Server login, which is used by Biometrics.
