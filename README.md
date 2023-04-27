![](https://i.imgur.com/b0ZyIx5.jpg)

Table of Contents
=======================
* [Project Outline](#project-outline)
* [Setting Up SSH](#setting-up-ssh)
* [Test Case 1](#test-case-1)
* [Test Case 2](#test-case-2)
* [Test Case 3](#test-case-3)

---

Project Outline
------

This capstone project aims to improve the level of autonomy in a 2023 Subaru Crosstreck while testing variations of the Open Pilot software. The team will give insights on what software and features enhance the experience of the daily commuter or anyone who finds themself frequently on the road. The report contains links to guides and repositories that we found valuable while working with OpenPilot. Along with testing variations of different software, the team will demonstrate how to adjust parameters in the code and test your own code changes. This project is a full product test on the Comma 3 while demonstrating our knowledge obtained while enrolled in the Data Science and Analytics Autonomous Vehicle Concentration at Ferris State University. 

Setting Up SSH
------
Generating the SSH key provides you with two keys, one public and one private. The public key is placed on the server and the server is connected using an SSH client which already has a private key configured. We used PuTTY as our Client and when both keys match up, you can log in to your server without the need for a password.

picture

Comma 3 devices allow Keys to be added using GitHub Usernames. So linking the new key to your GitHub needs to be done before enabling SSH on Comma 3. 

picture

With Comma Prime you will be able to enable SSH on the Comma device and use SSH Keys from your GitHub. Link your GitHub username on your comma device after enabling SSH. This is all done in the advanced settings on the Comma 3. Save the IP Address of the device as it is needed when configuring the connection to commit code changes. 

picture

Usings PuTTY to configure the SSH connection the Host Name is “comma@IP_ADDRESS”. Where “IP_ADDRESS” is the IP address from the advanced settings on the comma 3 device. The Port is left at the standard which is 22, and the private key is the file saved from the PuTTY key generator. 

picture

This means the configuration is set up correctly and the SSH connection is working properly. The computer is now connected to the Linux server running on the device and we are able to make parameter changes to perform our testing. After the commits have been performed run sudo reboot or unplug the device to reset the Comma system. You can also open a new SSH connection and open the file to verify the commits have been saved. 


Test Case 1
------

Test Case 2
------

Test Case 3
------

