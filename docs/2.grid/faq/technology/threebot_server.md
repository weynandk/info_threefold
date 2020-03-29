# How to deploy your own Threebot?

Prerequisites:
- You need to have an identity created by the 3bot login app.
- You shouldn't have any previous record in our phonebook.


To deploy a 3bot, go to http://explorer.testnet.grid.tf/chat. You will be asked to login using the 3bot login app.

![](img/login.png)

Now that your are logged in, click on the `Threebot deploy` button. This will open a chat bot that will guide you through the steps to create your 3bot.

![](img/selectchat.png)

Progress through the chatflow by pressing Next to start the deployment.

![](img/startdeployment.png)


You'll see some progress update while waiting for the deployment to finish. This may take a few minutes.
![](img/configuring3bot.png)


Once your 3bot is alive, click the link to finish the initialization of the 3bot.
![](img/botsuccess.png)


The first time you connect to your 3bot, a form will be presented so you can finish initializing your 3bot.
- Country: ...
- Referenced by: the "double name" of a eventual person that refereed you to intall a 3bot.
- Seed: this is the important part. To know your identity seed, open the 3bot login app, click on the gear on the top right side of the app to open the preference page.
then click `show phrase`. A pop up with your seed will be shown, copy this list of words into the form.

![](img/botlogin.png)


Your 3bot is now initialized. You can go to <3boturl>/packagemanagerui/ to enable/disable/install apps.

![](img/packagemanager.png)
