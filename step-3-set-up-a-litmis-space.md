# Step 3: Set up a LITMIS Space

Now that you know a little about PASE, it's time to set up your lab on an IBM i in the cloud. Labs are conducted on [**Litmis Spaces**](http://krengel.tech/spaces-litmis) **Multi Tenant**; a service from [Krengel Technology](https://www.krengeltech.com) to provide preconfigured open source environments on IBM i cloud instances.

**In short, everything can be done through the browser - no need to install a source editor or shell client on your desktop. Happy day!**

Go to [https://spaces.litmis.com](https://spaces.litmis.com) and select **SIGN UP**, as show below.

![](.gitbook/assets/spaces_signup.png)

Select the authentication mechanism of your choice. If you don't have an account with any of the options listed, you can register a free [Github.com](http://github.com) profile, and then return back to this page once your Github profile is set up.

![](.gitbook/assets/litmis_signup2.png)

Once logged in you can create a new space, as shown below.

![](.gitbook/assets/litmis_signup2.5.png)

You will be presented with the below pop-up. Give a name to this space, enter the promo code of **BETA**, select the `minimal` radio button, and click the **Create** button.

![](.gitbook/assets/litmis_signup3.png)

Now you should see a new box on your page that represents your newly created Space.

![](.gitbook/assets/litmis_space_minimal.png)

There are four buttons which constitute actions you can take with your Space. They are \(left to right\):

* **Shell.** You will use this to enter commands in the PASE environment on the IBM i. This takes the place of `STRQSH` and `CALL QP2TERM` mentioned earlier.
* **Editor.** Where you will edit your source code and navigate the IFS \(Integrated File System\).
* **Space Information.** Here you will find information about your Space such as user profile, database schemas \(aka libraries\), ports for your web app to listen, Space id, etc.
* **Delete Space.** **WARNING!** If you select this option and the subsequent warning prompt, your Space will be deleted. This **CANNOT** be undone.

## Please proceed to the next step.

