[title]: # (Using the App)
[tags]: # (mobile)
[priority]: # (3)
# Using the Application

The application will display the Secrets in a UI similar to the Basic dashboard in Secret Server. Clicking on
a Secret will expand it and show the Secret information. You will be able to edit and open the Secret in
browser. Clicking Edit allows you start editing the contents of the Secret.

The mobile app can be used to authenticate to a Secret Server instance (on-prem or cloud) and access secrets. The app has the ability to run the following actions for both Secrets and Folders:

* View, add, edit, delete
* Search based on:
  * Name
* Favorite
  * Users have access to their Favorites list as a separate tab and can favorite or un-favorite secrets, which is then synchronized between the mobile device and Secret Server and vice versa.
* Recent
  * Shows the user's 15 most recently accessed secrets.

Users access and use their secrets via mobile device, using the built-in password management features. When Users are logged in with their own account, users can navigate the Secret Server folder structure to access any of their Secrets.
The applications allows users to automatically fill credentials from Secrets into other mobile apps or Web browser sites on the mobile device. For this to work correctly, the application needs to be registered with the device's autofill service.

The application allows users to launch a web session from a Secret on the mobile device and have the credentials auto-populate in the mobile devices default browser.

## Navigating the Application

### Home Page

The Home page lets users browse existing and add new secrets.

![home](images/main.png "Home page")

Use the __+__ icon to add new secrets or folders to Secret Server.

![add](images/add.png "Add a Secret or Folder")

#### Ellipsis Options

Secrets and folders have ellipsis menu options that allow users to view, edit, and delete items based on permission levels. The options available are dynamic based on the Secret.

![ellipsis](images/ellipsis.png "Ellipsis Menu Options")

### Hamburger Menu

![hamburger](images/hamburger.png "Hamburger menu options")

#### Folders

The Folders page lets users access and browse existing folders and also add new folders for secrets.

![folders](images/folders.png "Folders page")

#### Change Password

The Change Password page uses the standard change password user flow asking for the existing password and then entering and confirming a new password.

![password](images/password.png "Change Password page")

#### Settings

The Settings page is used to enable/disable biometrics and autofill functionality for the mobile application.

![settings](../onboarding/images/init-5.png "Settings page")

#### Feedback

The Feedback page allows users to provide a review of their experience with our mobile application.

![feedback](images/feedback.png "Feedback page")

### Favorites

The Favorites lists the secrets marked as favorites in the mobile application. It also populates the information for favorites secrets from the Secret Server instance based on user.

![favorites](images/favorites.png "Favorites page")

### Recent

The Recent page provides the list of recently accessed/used secrets.

![recent](images/recent.png "Recent page")

### Shared

The Shared page provides the list of shared secrets.

![shared](images/shared.png "Shared page")

## Launching a Web Password Secret

Users can launch Web Secrets directly from the secret's details page.

![launch](images/launch.png "Launch web secret")

1. Click the launcher icon in the top right of the details page.

## Autofill

When the Autofill service is enable on the device, the Secret Server Mobile application works with the devices built-in autofill features to fill username and password fields for web pages or other mobile applications.

When you select the mobile application or web page and click on the username field you should see a prompt to use the autofill service from Secret Server Mobile. Clicking this option will open the app and (after logging in if needed) it runs a search of your secrets for:

* Browser web site - The search will be run looking for any secret that has the same Domain value in the URL
* Other mobile application - The search will run looking for any secret that has the same name or URL value as the name of the mobile application that is being filled.

Users can also choose to manually modify the search value and run it again. Once the list of Secret Server Secrets has been returned, you can select which one you want to use and the autofill service will fill those credentials in the related username and password fields.

>**Note**: Currently the autofill service only has support for username and password fields, and it does not fill in any other additional fields.
