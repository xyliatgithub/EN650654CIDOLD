# Lab 1 - Network Traffic Traffic & DoS Attack on GENI

In this lab, we will perform an experimental Denial-of-Service attack and collect network packets on the GENI testbed. First your request to join the class project needs to be approved by the instructor or CA. So please send out the request ASAP!!

## GENI 101

Please set up your GENI account ASAP. Go to [https://portal.geni.net] and log in with your JHU ID. You may need to search for "Johns Hopkins" the first time.
After you log into the GENI Portal, find Join the Project button and request to join the class project named "EN650654-2021". 
- Once you are approved to join the project, you can create your own experiment slices.
- For Windows users, please refer to these getting started series of [win-1](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedWindows.html) [win-2](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedWindowsHelloGENI.html).
- For Mac users, please refer to these guides [mac-1](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedMac.html) [mac-2](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedMacHelloGENI.html).

## Lab Instructions 

Please follow the instructions on [this page](http://mountrouidoux.people.cofc.edu/CyberPaths/networktrafficandddos.html) to complete the lab. In case the hyperlink does not work, here's the full URL: [http://mountrouidoux.people.cofc.edu/CyberPaths/networktrafficandddos.html]

**Note: A few changes are needed in order to successfully run this lab:**
- Setup: Step 5: Please use the new rspec file "denialOfServiceLevel1_NEW.txt" instead of the file at the given link. You can use the File option or copy the content of "denialOfServiceLevel1_NEW.txt" using the Text Box option.
- Setup: If you follow all the steps but your experiment does not start as expected, please check the error messages. Sometimes you need to try another aggregate since the resources at the slected aggregate are limited.
- Part 5: Step 5: If you are a Mac or Linux user and you cannot use SFTP to connect to the node successfully, you need to use your key like ssh. The command may look like: "sftp -i <your key for ssh> -oPort=<Your corresponding port from the previous step> your_username@host"
- After finishing the lab, please do not forget to delete the resources of your experiment so they become for other users.

## If You Need Help...

If there are any questions about getting started with GENI or working on the lab, feel free to send an email to the CA, Qingshan Zhang (qzhang68@jhu.edu)
