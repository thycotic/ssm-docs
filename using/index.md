[title]: # (Navigating the Mobile Application)
[tags]: # (mobile,interface,navigation)
[priority]: # (3)

# Navigating the Application

Through the Secret Server Mobile application, users can authenticate to a Secret Server instance and access secrets using built-in password management features. The mobile application displays secrets in an interface similar to the Secret Server interface.

Users can navigate in the mobile application to view secrets and secret folders. They can also add and delete secrets, as well as click on a secret to examine and edit it.

By registering Secret Server Mobile with a mobile device's autofill service, users can launch a web session from a secret on the mobile device and automatically populate login credentials on specified web sites.

## Navigating the Application

### Home Page

The Home screen offers several options enabling users to view secrets. The Search feature (magnifying glass icon) enables users to search for secrets by name. Four tabs on the Home page enable users to view four different subsets of secrets:

* **All**: all secrets the user has view access to

* **Favorites**: secrets the user has designated as "Favorite"

* **Recent**: the 15 secrets most recently used by the user

* **Shared**: secrets shared between the user and other users

![home](images/main.png "Home page")

Use the __+__ icon to add new Secrets or folders to Secret Server.

![add](images/add.png "Add a Secret or Folder")

#### Ellipsis Options

Secrets and folders have ellipsis menus offering options such as view, edit, favorite, and delete. 
The options available are dynamic, based on the Secret and the user's permission levels.

![ellipsis](images/ellipsis.png "Ellipsis Menu Options")

### Hamburger Menu

![hamburger](images/hamburger.png "Hamburger menu options")

#### Folders

The Folders page lets users access and browse existing folders, and add new folders for secrets.

![folders](images/folders.png "Folders page")

#### Change Password

The Change Password page uses the standard change password user workflow, asking for the existing password and then entering and confirming a new password.

![password](images/password.png "Change Password page")

#### Settings

The Settings page is used to enable/disable biometrics and autofill functionality for the mobile application.

![settings](../onboarding/images/init-5.png "Settings page")

#### Feedback

The Feedback page allows users to provide a review of their experience with the Secret Server Mobile application.

![feedback](images/feedback.png "Feedback page")

### Favorites

The Favorites page displays secrets the user has marked as favorites. It also populates the information for favorites secrets from the Secret Server instance based on user.

![favorites](images/favorites.png "Favorites page")

### Recent

The Recent page displays the Secrets the user has recently accessed or used.

![recent](images/recent.png "Recent page")

### Shared

The Shared page displays shared Secrets.

![shared](images/shared.png "Shared page")


Some Secrets, especially Secrets that are shared across an organization, require the user to request and receive approval to access the Secret. During the process of requesting approval to access a Secret, the user can be prompted to enter security information such as a comment, ticket number, reason, or Double Lock password, and to check out the secret for their personal use for a specified period. The screen shots below show the sequence for specifying a check out period through the Request Approval, Select Duration, and Custom screens. 


On the **Request Approval** screen, the user clicks to enter the duration value. Note that some scrolling-down might be required.

![request](images/request-approval-duration2.png "Request Approval")


On the **Select Duration** screen, the user chooses a preset duration or chooses **Custom**. If the user chooses **Custom**, the Custom screen appears.

![duration](images/select-duration2.png "Select Duration")



On the **Custom** screen, the user clicks to enter the duration value. Note that some scrolling-down might be required.


![custom](images/duration-custom2.png "Custom Duration")


Secrets that are already checked out are marked as **Checked Out**.

![checked out](images/secret-checked-out2.png "Checked Out")


## Launching a Web Password Secret

Users can launch Web Secrets directly from the Secret's details page.

![launch](images/launch.png "Launch web secret")

1. Click the launcher icon in the top right of the details page.

