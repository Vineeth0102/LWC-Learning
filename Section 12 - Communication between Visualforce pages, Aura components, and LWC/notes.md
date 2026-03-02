Lightning Messaging Service
    LMS is the first Salesforce technology which enables you to communciate between Visualforce, Aura component and Lightning web component anywhere in lightning pages including utility components.<br><br>
    In Winter 20, Salesforce is released "Lightning Message Service" (LMS)
    ![alt text](image.png)<br><br>
    Prerequisite to create the message channel
        1. Create a folder called messageChannels under the path force-app\main\default
        2. create a file CHANNELNAME.messageChannel-meta.xml inside the folder
        ![alt text](image-1.png)
        3. Add following XML definition to message channel file
        ![alt text](image-2.png)
        4. Update the manifest/package.xml file by adding the LightningMessageChannel
        ![alt text](image-3.png)
        5. API Version should be above 47 & above<br><br>
    LWC to LWC Communication using LMSs
    ![alt text](image-4.png)
    ![alt text](image-5.png)<br><br>
    LWC To AURA Communication using LMS
    ![alt text](image-6.png)
    LWC to VisualForce Page Communication using LMS
    ![alt text](image-7.png)
