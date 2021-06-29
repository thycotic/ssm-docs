[title]: # (Configuring Secret Server for the Mobile Application)
[tags]: # (mobile,web services,offline caching)
[priority]: # (2)

# Configuring Secret Server for the Mobile Application

Before you can use the Secret Server Mobile application, a Secret Server administrator must make the following configurations in Secret Server:

## Enable Web Services

Webservices must be enabled to allow communication via RestAPI between Secret Server and the mobile clients. See [Enabling Web Services](https://docs.thycotic.com/ss/10.9.0/webservices/enabling-webservices/index.md) in the Secret Server documentation for more information.

## Set Time Limits for Offline Caching and Web Services

For maximum security, do not choose Unlimited for session timeout, and restrict offline access to just a few days. See [Setting Maximum Time for Offline Caching](https://docs.thycotic.com/ss/10.9.0/mobile/maximum-offline-caching/index.md) in the Secret Server documentation for more information.

Secret Server administrators can check the mobile application onboarding progress in Event Pipelines. See [Event Pipelines](https://docs.thycotic.com/ss/10.9.0/events-and-alerts/event-pipelines#event_pipelines) in the Secret Server documentation for more information.
