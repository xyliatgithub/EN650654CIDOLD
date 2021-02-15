# Lab 2 - Local DNS Attack

In this lab assignment, you will need to setup multiple SEED lab VMs and perform the DNS attack. In addition to those tasks required by the SEED lab documentation, you also need to finish the additional tasks described below.

## Setup 

Go to  http://www.cis.syr.edu/~wedu/seed/lab_env.html to install the pre-built VM image (Ubuntu 16.04 32 bits).  

•	VM setup instruction (in Virtualbox): http://www.cis.syr.edu/~wedu/seed/Labs_16.04/Documents/SEEDVM_VirtualBoxManual.pdf  
•	Network Configuration: http://www.cis.syr.edu/~wedu/seed/Documentation/VirtualBox/VirtualBox_MultipleVMs.pdf  
•	User manual (contains the usernames and passowrds): http://www.cis.syr.edu/~wedu/seed/Documentation/Ubuntu16_04_VM/Ubuntu16_04_VM_Manual.pdf  

In this lab, you need to have three VMs under the same local network. Note that these three VMs should be in the promiscuous mode in order to listen to traffics from other VMs. 
Once you have configured a VM, you can simply clone that VM for two more times to complete the VM setup.   


## Lab Instructions

1. Please follow the instructions in the DNS_Local PDF file to complete all the 9 tasks. The first three tasks are basically the environment and DNS setup.   
•	Note: You will not be able to complete all the tasks without proper setup. So, if you encounter any problem, please reach out to the CA for help ASAP. 
 
2. You need to fulfill some required additional tasks.  
•	In Task 5 - Directly Spoofing Response to User, use tcpdump on the "User" machine to capture all the DNS packets.  
•	Since you know the IP address of the local DNS server, if there are any DNS responses that are NOT coming from the DNS server, then those DNS responses might be the spoofed packets coming from the attacker. Are you able to use tcpdump to specifically capture those spoofed DNS packets?  Explain why or why not clearly. If not, how do you detect such attacks that may include additional processing steps? Please specifically describe your attempts.  


## Report Submission
•	The lab is due on 2/28 (Friday) by 11:59 pm.  
•	You can work in a group up to two people (No exception for this lab as we have 18 students in this class now). Each group only needs to submit one report in PDF format.  
•	Complete all the tasks and write a detailed report with adequate screenshots and explanations.  

## Grading

•	50 pts  
•	Completeness (30 pts): All the steps as instructed in the lab manual must be included in the report with adequate evidence.  
•	Presentation (20 pts): The report must be clear and correct in organization and writing with adequate explanation.  

## If You Need Help...

If there are any questions, feel free to send an email to Qingshan Zhang (qzhang68@jhu.edu).