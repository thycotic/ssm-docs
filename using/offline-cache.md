[title]: # (Using Secrets from an Offline Cache)
[tags]: # (mobile,cache,offline)
[priority]: # (600)

# Offline Caching

Mobile devices and applications can lose internet connectivity for a number of reasons. When Secret Server Mobile loses internet connectivity, users cannot access their secrets directly from Secret Server. But an organization can permit its Secret Server Mobile users to save secrets and secret folders to an offline cache. Offline caching stores secrets, secret folders, and all of their associated data to a password-protected, encrypted data file. When a network connection to Secret Server is unavailable, users can access secrets and folders cached offline for a maximum Time-To-Live (TTL) period. TTL and access to offline caching are controlled by an organization’s Secret Server administrator globally, for all mobile devices in the organization. If an organization does not allow offline caching, the administrator sets the TTL to zero.

Accessing secrets saved to an offline cache requires using biometric face or fingerprint recognition. The offline cache is automatically updated by default, but a user can turn off the auto-update feature. The offline cache is automatically cleared when the user logs out of the application or switches to another user identity.

# Select Secrets to be Available Offline

To select secrets to be available in an offline cache, follow the procedure below

1. Connect to Secret Server

1. Select a secret or secret folder and click the ellipses on the side.

1. Select the **Cache Secret** option.

   ![home](images/cache-secret.png "Select Cache Secret")

## Identify Cached Secrets

When you have secrets saved to offline cache, they are marked with a "Cached" tag for easy identification.

![home](images/cache-tagged.png "Identify Cached Secrets")

Cached secrets whose time has expired are marked with an "Expired" tag.

![home](images/expired-cached.png "Expired Cached Secrets")

## See How Much Time Remains for Accessing Secrets in the Offline Cache

WHen you open a secret, the time remaining until expiration is shown at the top of the screen. The default background is black.

![home](images/expires-24-hours.png "Time to Expiration")

Wen the secret has just 24 hours or less until expiration, the background changes to red for easy identification.

![home](images/expires-23-hours.png "Less than 24 Hours to Expiration")
