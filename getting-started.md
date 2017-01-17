# Getting Started

## 1. Create a User Account

Go to [https://app.konstru.com/](https://app.konstru.com/) and sign up with your email address. The Konstru web application works best in the Google Chrome browser. Firefox and Internet Explorer are also supported.

## 2. Create a Project

//needs image

The first step in working with Konstru is the creation of a Konstru Project at [https://app.konstru.com/](https://app.konstru.com/). Click the large green button to create a new project. Choose a name and description for your project. In the demonstration below, we have named the project _Large Tower_.

**Project Name:** Your project name should be a high level designation, such as the name of the actual project as you refer to it in your work.

**Project Description:** Give your project a short meaningful description, so that when you share and collaborate, your colleagues will have a greater understanding of what the project is.

When you create a new project, Konstru automatically creates a new model named _Master Model_.

Once you've created a new Project, you are now able to upload a Model. This step is done from one of the Konstru plugins to upload the model from your computer. Generally speaking, your first Project upload will be to the _Master Model_, giving your _Master Model_ it's first _Version_.

## 3. Upload a Model

![](/assets/04.png)  
Konstru uses the same user interface for each of the seven desktop apps \(plugins\). To launch the desktop app, you should first review the installation section of this document to ensure Konstru will be available to you. Please note that we are continually updating our list of plugins to add more and more Konstru integrations! Once your plugin is installed, you will be able to launch the Konstru app directly from your modeling software \(see **Installation** section above for toolbar specific button locations\). Note that the Konstru plugin for RAM runs as an external .exe file, and requires no installation \(and thus also wont be found in the RAM toolbar, as it is run from it's Start Menu location\).

Once you have the desktop application open \(in this example, Revit\), select the project, and then the model \(_Master Model_\). Then press _Select Model_.

_Note: If you've only just created the Project, you may need to refresh the desktop side user interface for the Project you've created to appear in the list of your Projects._

In the next dialog box, double-check the name of the project and model \(1\) and then press _Update Konstru_ to upload the model to the Konstru database.

When prompted with additional dialogs, press _OK_.

_Note: If the Project/Model indicated in user interface \#1 below is incorrect, you will need to use the 'Change Model' button, which will redirect you to the previous Konstru window which lists your available Projects. Choose the correct Project and Model \(as per \#3. 'Upload a Model'\) then 'Select Model' to be directed back to the up/down interface._

![](/assets/05.png)

### What just happened \(Upload Staging\) / What's about to happen? \(Download Staging\)

These two questions are asked by many users, and Konstru answers them via two steps in the process which are discussed in \#5 + \#6: 'Staging' and 'Model Review'. The goal of these two steps is to give the user more detail about the data that is being transferred from your platform to Konstru and from Konstru to your platform. Staging specifically allows the user to cancel the upload/download before making any changes to either the Konstru model \(on upload\) or to their local platform model \(on download\).  
![](/assets/staging.png)

## 5. Staging

Staging takes place on both upload and download, and allows the user to review the objects that are part of the specific upload/download before actually making the changes to the Konstru model \(via an upload\) or changes to your local model \(via a download\). The user can prevent individual changes to objects by unchecking the 'Apply' button, or stop the process all together with the 'Cancel' button.

The key value identified in the Staging window is the 'Status' of an object. Below are the definitions of the various statuses in this interface:

* **NEW**: Object is being added to Konstru/Platform model for the first time.
* **UPDATED**: Object that was already present in Konstru/Platform and has had some attribute \(geometric or otherwise\) altered by the last Konstru operation. Updated objects.

* **DELETED**: Object that was present in Konstru/Platform before the update, but which during the update was not part of the data, and hence is about to be deleted.

![](images/GettingStarted/staging window with callouts.png)

Once the _Update Konstru Model_ process is complete, you can head directly to the web UI to review what was just added to your _Master Model_.

As you open the Project in the web interface, you will see that the _Master Model_ now contains one version. We just created our first version of this model! Every time we upload a subsequent version to this _Master Model_ we will be adding new _Versions_ to the Konstru Model. Each of those versions is captured so that users can view the entire history of any given model.

## 6. Model Review

Model Review with the Konstru webpage is two-fold. First, when opening a model, the user is presented a tabular report about  the contents of last update to the Model, whether objects were added, deleted, updated, or unchanged, and the total number of changes per object type. Users can then drill down into the type of change that was made, and still further into the actual list of changes by object type. Second, you are able to access a 3D preview of the updated model directly from the Report interface.

When reviewing large models, it is useful to limit the scope of area, or object type, that you wish to review. In Konstru, these tools are available to you for both Report Review and 3D View via the 'Details' interface, and include the ability to limit the vertical range of objects \(via 'Crop'\), toggle on or off the object types being reported/displayed \(via 'Type'\), and toggle on or off objects by their 'Status'.

For more details on Model Review, please view the **Tutorials** section.

## 7. Add Collaborators

If you want to share a project with a colleague or client, you can add 'Collaborators' in the _Project Settings_ tab under _Collaborators_. Collaborators to a Konstru project are users that did not create the Project but have certain permissions to interact with the Models and Versions that exist within a Project.

Users choose the permission levels of Collaborators. Collaborators can be allowed to \(1\) control the project \(_admin_\), \(2\) up/download models \(_write_\), or \(3\) view models \(_read_\). More info on permissions [here](the_web_user_interface.md).

**To add Collaborators to a Project**: Open your Project, then access the _Project Settings_ interface as seen below. Type in the email of the person you wish to add. If the person already has a Konstru account, select them from the drop-down. If the person does not have a Konstru account, you will have to enter their name and email. The next step is to define the Permissions level for the collaborator \(see above\)...and then press _Save_.

The user will receive an email invite to join your project on Konstru.

![](images/GettingStarted/GS_Collabs.png)

## 8. Download the model to a different application

Launch the Konstru plugin from a different desktop application and select the ![](images/GettingStarted/desktop_download.PNG) button. You should first check that the correct Project and Model are listed in the user interface, and, if necessary, use the 'Change Model' button. Second, you should review the specific Version you are about to download from the dropdown menu and make sure that the 'Delete Existing Elements' button is **unchecked**.

![](/assets/DownloadSteps.png)

'Delete existing elements' refers to objects that may be present in the platform model you are about download to, but are not part of the Konstru model you have chosen to download. Almost certainly there will be objects present in your platform model that are not present in the Konstru model \(tags, etc\); therefore, you will want to make sure those elements are not deleted by unchecking this box.

**Note**: Even if you forget to uncheck the "Delete Existing Elements" button, you can prevent the changes from overwriting your model by canceling the import at the 'Staging' window.

