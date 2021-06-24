[title]: # (1.6.0 Release)
[tags]: # (release notes)
[priority]: # (10995)

# 1.6.0 Release Notes

#### Release Date: July 6, 2021

## Feature Updates and Enhancements

* An organization can permit its Secret Server Mobile ("mobile app") users to save secrets to an offline cache. When a network connection to Secret Server is unavailable, users can access secrets cached offline for a specified Time-To-Live (TTL) period. TTL and access to offline caching are controlled by an organization’s Secret Server administrator globally, for all mobile devices in the organization. Accessing secrets saved to an offline cache requires using biometric face or fingerprint recognition. If an organization does not allow offline caching, the administrator sets the TTL to zero. More information on offline caching is available in the [publications set](https://docs.thycotic.com/ss/10.9.0/mobile/maximum-offline-caching/index.md).

* Secret Server Mobile now permits Android users to log into Secret Server using a self-signed or internal certificate that cannot be validated by a third party or CA. Because this process bypasses CRL checking it is appropriate only for Proofs of Concept and other closed environments. It is not appropriate for production environments or other environments exposed to incoming internet traffic. The mobile app displays a warning that the certificate cannot be validated with any CRL servers and that bypassing the CRL check may be harmful. The user can connect to Secret Server only if they acknowledge that they have read the warning and that they choose to proceed anyway at their own risk. The option to bypass CRL checking is not available on iOS devices.

## Bug Fixes

* Radius authentication issues in the mobile app have been resolved in the current release.

* A user accessing a secret protected by the workflow, "Viewing Password Requires Edit," can now auto-fill their credentials without error, using a launcher or using web login credential fields that display the Thycotic logo. The mobile application still bars users from viewing the password and from copying or pasting it using the clipboard function.

## Known Issues

The mobile app does not support the following secret templates, and using them in SSM will result in errors:

* Google IAM Service Account
* Unix Account SSH Key Rotation - No Password
