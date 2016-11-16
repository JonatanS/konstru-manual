# Desktop Clients

## Upload a Model to TTX-Cloud

## Download a Model from TTX-Cloud to a desktop app
Every platform has the same UI. Once you click TTX 0.5 it will either prompt you to select a model or remember the model you selected last time. The screenshot below shows the key features of the Up/Download dialog:

![](images/UI/UpDownloadDialog.png)
After clicking Up or Download the process is always the same. TTX will compare the model on the server against the model you are about to upload or download to and display the changes in the staging UI.
## The Staging UI
The staging UI tells you about the differences between your local model and the model on the server. It brings transparency by previewing each change that is going to happen. You can review the changes that are about to happen element by element. Every line represents one element. If you are in doubt or don't want to perform any changes you can click Cancel to stop the process.

![](images/UI/StagingWindow.png)
The Status column is telling you about the action TTX will perform. Adding, Deleting or Updating a single element. The 5 columns called change (Name change, etc - highlighted in red above) are telling you about each change in detail. In the example above 3 columns will change their profile to 24". 