# Lab 1 - Network Traffic & DoS Attack on GENI

In this lab, we will perform an experimental Denial-of-Service attack and collect network packets on the GENI testbed. First your request to join the class project needs to be approved by the instructor or CA. So please send out the request ASAP!!

## GENI 101

Please set up your GENI account ASAP. Go to [https://portal.geni.net] and log in with your JHU ID. You may need to search for "Johns Hopkins" the first time.
After you log into the GENI Portal, find Join the Project button and request to join the class project named "EN650654-2021". 
- Once you are approved to join the project, you can create your own experiment slices.
- For Windows users, please refer to these getting started series of [win-1](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedWindows.html) and [win-2](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedWindowsHelloGENI.html).
- For Mac users, please refer to these guides of [mac-1](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedMac.html) and [mac-2](http://mountrouidoux.people.cofc.edu/CyberPaths/GettingStartedMacHelloGENI.html).

## Lab Instructions 

Please follow the instructions on [this page](http://mountrouidoux.people.cofc.edu/CyberPaths/networktrafficandddos.html) to complete the lab. In case the hyperlink does not work, here's the full URL: [http://mountrouidoux.people.cofc.edu/CyberPaths/networktrafficandddos.html]

**Note: A few changes are needed in order to successfully run this lab:**
- Setup: Step 5: Please use the new rspec file "denialOfServiceLevel1_NEW.txt" instead of the file at the given link. You can use the File option or copy the content of "denialOfServiceLevel1_NEW.txt" using the Text Box option.
- Setup: If you follow all the steps but your experiment does not start as expected, please check the error messages. Sometimes you need to try another aggregate since the resources at the selected aggregate are limited.
- Part 5: Step 5: If you are a Mac or Linux user and you cannot use SFTP to connect to the node successfully, you need to use your key like ssh. The command may look like:  
" sftp -i \<the same key with your ssh key\> -o Port=\<Your corresponding port from the previous step\> your_username@host "
- Part7: You could only analyze the regular traffic. Just repeat step1-3 from Part5 four more times. Use iperf to generate traffic and use tcpdump to generate pcap files. You do not need to attack. Notice that you should make each traffic generation time as same as possible.  
To control the time more accurately, You could use the following command:  
"sudo tcpdump -i <interface> -s0 -G <the time you want> -w %H%M_%S.pcap"  
Notice: Do not set the time too long in case the Pcap file will be too large.
- After finishing the lab, please do not forget to delete the resources of your slice so they can be used by other users.
