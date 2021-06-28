[title]: # (Troubleshooting)
[tags]: # (mobile)
[priority]: # (4)

# Troubleshooting for Secret Server Administrators

If a user is unable to connect to their Secret Server instance from Secret Server Mobile, please check the following:

* If the Desktop Client is not starting, or if the user receives a **Login Failed** error with correct credentials, you may need to uninstall and re-install Java.

* Are you using SSL? If so, is your certificate trusted? Check with your IIS administrator to get a valid certificate.

* Are webservices enabled? Go to **Administration \> Configuration** and ensure that **Enable Webservices** is set to **Yes**.

<!--1. Are you using Integrated Windows Authentication?
   * Please refer to the steps in this KB article for enabling mobile access in this case. -->

* Check the URL being used for the mobile application - it should be the URL of the Login.aspx without 'login.aspx'. For example:

   * For `https://secretserver/ss/Login.aspx`, use this URL: `https://secretserver/ss`
   * For `https://secretserver/Login.aspx`, use this URL: `https://secretserver/`
   * For `http://ss.myserver1.com/Login.aspx`, use this URL: `http://ss.myserver1.com/`
