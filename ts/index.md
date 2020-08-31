[title]: # (Troubleshooting)
[tags]: # (mobile)
[priority]: # (4)
# Troubleshooting

If you are unable to connect a client application or mobile device to your Secret Server instance please check the following:

If the Desktop Client is not starting or you are receiving a Login Failed error with your correct credentials you may need to uninstall and re-install Java.

For example:
* `https://secretserver/ss/Login.aspx` the URL to use is `https://secretserver/ss`
* `https://secretserver/Login.aspx` the URL to use is `https://secretserver/`
* `http://ss.myserver1.com/Login.aspx` the URL to use is `http://ss.myserver1.com/`

1. Are webservices enabled?  
   * Go to Administration->Configuration and ensure that "Enable Webservices" is set to "Yes".
<!--1. Are you using Integrated Windows Authentication?
   * Please refer to the steps in this KB article for enabling mobile access in this case. -->
1. Can you browse to Secret Server from the mobile device? If you are unable to browse to the Secret Server site using your mobile web browser, then that means that Secret Server is unreachable from your device. Ensure that you are on the wireless intranet, or that the Secret Server site is available from outside your internal network.
1. Check the URL you are using on the client application or mobile device - it should the URL of the Login.aspx without login.aspx
1. Are you using SSL? If so, is your certificate trusted? Check with your IIS administrator to get a valid certificate (More details in this KB article).
1. A "you don't have permissions" message is usually due to workflows on the secret.
