![](https://i.imgur.com/b0ZyIx5.jpg)

Table of Contents
=======================
* [Project Outline](#project-outline)
* [Setting Up SSH](#setting-up-ssh)
* [Commit Code Changes](#commit-code-changes)
* [Making Changes to Files in OpenPilot](#making-changes-to-files-in-openPilot)
* [Test Case 3](#test-case-3)

---

Project Outline
------

This capstone project aims to improve the level of autonomy in a 2023 Subaru Crosstreck while testing variations of the Open Pilot software. The team will give insights on what software and features enhance the experience of the daily commuter or anyone who finds themself frequently on the road. The report contains links to guides and repositories that we found valuable while working with OpenPilot. Along with testing variations of different software, the team will demonstrate how to adjust parameters in the code and test your own code changes. This project is a full product test on the Comma 3 while demonstrating our knowledge obtained while enrolled in the Data Science and Analytics Autonomous Vehicle Concentration at Ferris State University. 

Setting Up SSH
------
Generating the SSH key provides you with two keys, one public and one private. The public key is placed on the server and the server is connected using an SSH client which already has a private key configured. We used PuTTY as our Client and when both keys match up, you can log in to your server without the need for a password.

![1](https://user-images.githubusercontent.com/24868690/235015644-6e396917-580d-490f-bd8d-beb2f0df0dfb.PNG)


Comma 3 devices allow Keys to be added using GitHub Usernames. So linking the new key to your GitHub needs to be done before enabling SSH on Comma 3. 

![2](https://user-images.githubusercontent.com/24868690/235015019-e7c853ec-aa5c-48d0-b11c-c8289cab3127.PNG)


With Comma Prime you will be able to enable SSH on the Comma device and use SSH Keys from your GitHub. Link your GitHub username on your comma device after enabling SSH. This is all done in the advanced settings on the Comma 3. Save the IP Address of the device as it is needed when configuring the connection to commit code changes. 

![3](https://user-images.githubusercontent.com/24868690/235015157-2571ed04-ea24-4ea2-85ab-246ad1f3c90c.PNG)


Usings PuTTY to configure the SSH connection the Host Name is “comma@IP_ADDRESS”. Where “IP_ADDRESS” is the IP address from the advanced settings on the comma 3 device. The Port is left at the standard which is 22, and the private key is the file saved from the PuTTY key generator. 

![4](https://user-images.githubusercontent.com/24868690/235015406-c403fb3d-c7ca-4a67-a243-d44964959d3a.PNG)

![5](https://user-images.githubusercontent.com/24868690/235016293-e723b2d0-8803-4f4c-a39c-7d3576cd1fd8.PNG)

This means the configuration is set up correctly and the SSH connection is working properly. The computer is now connected to the Linux server running on the device and we are able to make parameter changes to perform our testing. After the commits have been performed run sudo reboot or unplug the device to reset the Comma system. You can also open a new SSH connection and open the file to verify the commits have been saved. 


Commit Code Changes
------

![7](https://user-images.githubusercontent.com/24868690/235017980-75be3cf2-5a87-4ed4-a347-a09fe6e14d8f.PNG)

![8](https://user-images.githubusercontent.com/24868690/235018003-ae5c2290-ff9d-4293-8f3d-f81ccb8ff7f1.PNG)

This means the configuration is set up correctly and the SSH connection is working properly. The computer is now connected to the Linux server running on the device and we are able to make parameter changes to perform our testing. After the commits have been performed run sudo reboot or unplug the device to reset the Comma system. You can also open a new SSH connection and open the file to verify the commits have been saved.

Making Changes to Files in OpenPilot
------

![20](https://user-images.githubusercontent.com/24868690/235018972-e43f6587-28e5-458a-b994-646ecaa3cc3d.PNG)

This is an example of how to navigate through the code running on the Comma 3. ls and cd commands are very common when working with Linux systems. 
The teams tested parameters for this project were all done in the following file:

“openpilot/selfdrive/modeld/models/driving.cc”

![21](https://user-images.githubusercontent.com/24868690/235020061-590b50c8-12b7-4359-a663-7e100122bbad.PNG)

When changing the code using “SUDO VIM” all file changes are keyboard based. A Guide our team found useful was for VIM commands:

