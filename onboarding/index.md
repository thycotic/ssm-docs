[title]: # (Prerequisites and Requirements)
[tags]: # (mobile,prerequisites,compatibility)
[priority]: # (3)

# Prerequisites and Requirements

## Secret Server Prerequisites

Before you can use the Secret Server Mobile application, an administrator must configure Secret Server for web services with time limits and must configure time limits for offline caching.

### Enable Web Services with Time Limits in Secret Server

To allow communication via RestAPI between the mobile application and Secret Server, Webservices must be enabled in Secret Server. For maximum security, do not set session timeout to "Unlimited." See [Enabling Web Services](https://docs.thycotic.com/ss/10.9.0/webservices/enabling-webservices/index.md) in the Secret Server documentation for more information.

### Set Time Limits for Offline Caching in Secret Server

To use offline caching in the mobile application, an administrator must configure offline caching Time to Live (TTL) in Secret Server. Administrators can disable offline caching globally by setting the TTL to zero. For maximum security, restrict offline access to no more than a few days. See [Setting Maximum Time for Offline Caching](https://docs.thycotic.com/ss/10.9.0/mobile/maximum-offline-caching/index.md) in the Secret Server documentation for more information.

Secret Server administrators can check the mobile application onboarding progress in Event Pipelines. See [Event Pipelines](https://docs.thycotic.com/ss/10.9.0/events-and-alerts/event-pipelines#event_pipelines) in the Secret Server documentation for more information.

## Requirements

### Operating System Requirements

The following Operating Systems are supported:

* iOS 12 and up
* Android 8 and up

### Minimum Hardware Requirements

Mobile devices not more than four years old running operating systems as described above.

### Compatibility Requirements

The Secret Server Mobile Application works with Secret Server on-premises and cloud instances starting with Version 10.8 and up. To utilize Secret Server's __onboarding feature__, Secret Server 10.9 is a minimum requirement.

Offline Caching requires Secret Server 10.9.000064 or higher.

The mobile application integrates via Secret Server's RESTApi.
