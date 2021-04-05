# Lab 4 - Intrusion Detection Systems on GENI

In this lab assignment, you will set up an environment on GENI to get familiar with the intrusion detection system of Snort. 

**Basic Tasks**  
Follow this document (http://mountrouidoux.people.cofc.edu/CyberPaths/IntrusionDetectionSystemLabEasy.html) and complete Part 1 to Part 4. 


## Additional Tasks  
### 1. Get more familiar with Snort commands  
1.1 Based on the command you run in the above document, you shall not be able to see alerts on the console prompt to run Snort. The actual alert log file will be stored under the /var/log/snort directory. However, if you try to read that log file, you will see some gibberish instead of some meaning alert messages. Do some googling or read through a few online tutorials about Snort to see if you're able to figure this out. (Hint: you have probably done this in Lab 1.)  
1.2 Try to add a new option in the Snort command to make the stored alert log files being readable by human being, a.k.a. ASCII mode.  
1.3 Modify the Snort command so that the alert messages can be shown up on the console prompt instead of being stored.  
1.4 Take a look at the pre-installed Snort rules (/etc/snort/rules). Find out where the rule is that can detect the SYN flooding attack, and explain your finding and this rule. Please test it to detect the attack in Part 4.  

### 2. Create new rules  
If you want to create new rules, the new rules should be stored in /etc/snort/rules/local.rules. Once you update the rules, always run the command "sudo snort -c /etc/snort/snort.conf -T -i eth1" to make sure there's no syntax error. Remember that you should always show how these rules work and include necessary screenshots.  
2.1 Please create a custom rule that can detect SSH connections on the Monitor node.  
2.2 Install "nmap" on the Attacker node. Try three different types of nmap scanning of the Victim node, and create customized Snort rules to detect such nmap scanning.  
2.3 Are you able to create a Snort rule to detect the "failed login attempt of SSH connection"?  Explain why or why not clearly.

### 3. slowloris attack detection  
3.1 Study the slowloris code (https://github.com/gkbrk/slowloris/blob/master/slowloris.py). Explain how this attack is done and its potential impact on a victim.  
3.2 Please create a custom rule that can detect this attack on the Monitor node.  
3.3 Test your alert by running slowloris code to see if your rule worked.
