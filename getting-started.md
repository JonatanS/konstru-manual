#Getting Started

##1. Create a User Account
Go to **https://ttx-webapp.herokuapp.com/** and sign up with your TT email address.
The TTX-Cloud web application works best in a Chrome browser, but also in Firefox and Internet Explorer (IE being the slowest of the three).

##2. Create a Project
![](images/GettingStarted/GS_createProject1.PNG)
Before you are able to do anything with TTX cloud you must create a TTX Project. This is done directly from the web address listed above (**https://ttx-webapp.herokuapp.com/** ).

Click the large green button to create a new project. Choose a name and description. For this demo, I name the project *Large Tower*.

**Project Name:** Should be a high level designation, such as the name of the TT Project. Analogous to the TT Project Number.

**Project Description:** A short meaningful description. 

When you create a new project, a new model named *Master Model* is automatically created.

Once you've created a new Project, you are now able to upload a Model. This step is done via the desktop  side of things.

##3. Upload a Model
![](images/GettingStarted/GS_desktopUI.png)
TTX-Cloud uses the same UI for each of the seven desktop apps. To launch the desktop app you should first review the installation section of this document to ensure TTX-Cloud will be available to you. Once installed, you will be able to launch the TTX-Cloud app directly from your platform (see installation for toolbar specifics). Note that TTX-Cloud RAM runs as an external .exe file, and requires no installation (and wont be found in the RAM toolbar). 

Once you have the desktop application open (in my case Revit), select the project, and then the model (*Master Model*). Then press *Select Model*.

*Note: that if you've only just created the Project, you may need to refresh the desktop side user interface for the Project you've created to appear in the list of your Projects.*

In the next dialog box, double-check the name of the project and model (1) and then press *Update TTX* to upload the model to the TTX-Cloud DB.
When prompted with additional dialogs, press *OK*.

*Note: If the Project/Model indicated in 1. below is incorrect, you will need to use the 'Change Model' button, which will redirect you to the previous TTX-Cloud window which lists your available Projects. Simply choose the correct Project and Model (as per #3. Upload a Model) then 'Select Model' to be directed back to the up/down interface.* 

![](images/GettingStarted/GS_desktopUI2.png)

When you now enter the project in the web UI, you will see that the *Master Model* contains one version now. We just created our first version of this model. Every time that we make changes to it, a new version is added for this model. 
##4. Add Collaborators
If you want to share this project with anybody, you can add a collaborator in the *Project Settings* tab  under *Collaborators*.
Type in the email of the person to add. If the person already has a TTX-Cloud account, select them from the drop-down. Else, you'll have to fill out their name and email. Then press *Save*. 
The user will receive an email invite to join your project.

Choose your permission levels depending on whether you want them to control the project (admin), up/download models (write) or just view models (read). More info on permissions [here](the_web_user_interface.md).
![](images/GettingStarted/GS_Collabs.png)

##5. Download the model (to a different application)
Launch the TTX-Cloud plugin from a different desktop application and select the ![](images/GettingStarted/desktop_download.PNG) button.

