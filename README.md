This assignment will be completed using the Damn Vulnerable Web App (DVWA) which is already installed on your Ubuntu VM.  You can access it by opening up a web browser, load the web site that is running on your Ubuntu VM and then clicking “Damn Vulnerable Web App” under the “Additional items to hack” section.

When you first load the DVWA site you will see a “Database Setup” page.  Everything is ready to go, you just need to scroll down to the bottom and click the “Create / Reset Database” button at the bottom.  Click the button and DVWA will complete the setup and take you to the DVWA login page.  The login information is:

User: admin

Password: password

 

## Login and complete the 4 challenges below:

 

### File Inclusion
Click the File Inclusion tab on the left.  Review the page and determine how to access and display the /etc/passwd file.  The Linux Primer can be helpful if you are unfamiliar with the Unix file system tree and how to navigate directories.

- Provide the URL you used to show the /etc/passwd file
- Provide a screenshot of the output from the page showing the /etc/passwd file
 

### SQL Injection
Click the SQL Injection tab on the left.  Review the page and determine how to inject SQL commands into the page.  Your end goal will be to list all of the users (there are 5) with a single SQL command.

- Provide the SQL query you injected into the page to list all of the users
- Provide a screenshot of the output from the page showing all of the users
 

### File Upload
Click the File Upload tab on the left.  Review the page.  Create a webshell (review the in-class Exercise on Weevely) and upload a Weevely webshell.  Access the webshell via Weevely and run the id command.

- Provide a screenshot of your active Weevely webshell session showing the full URL of your webshell on the Ubuntu host and the output of the id command.
 

### Command Injection
Click the Command Injection tab on the left.  Review the page and determine how you can run arbitrary commands with it.  Use Metasploit to generate a Meterpreter listener, the command to connect to it and use these to open a Meterpreter shell on the Ubuntu system. Once connected use the sysinfo Meterpreter command and take a screenshot of the output of this command.

Some helpful information for this step:

1. The Metasploit exploit to use is exploit/multi/script/web_delivery
2. DVWA uses PHP so the target to use is PHP
3. The payload to use is php/meterpreter/reverse_tcp
4. Provide a screenshot of your Metasploit session showing everything from your selection of the exploit to run, and the exploit command showing the command to run on the target machine
5. Provide a screenshot of your Meterpreter session showing the output from sysinfo.
   
