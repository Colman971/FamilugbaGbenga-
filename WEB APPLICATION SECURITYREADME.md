CYBER SECURITY INTERNSHIP REPORT

TASK 2 OVERVIEW
Web Application security
Objective:
Practical Illustration how web applications vulnerabilities can be analyzed and how attackers exploit weak vulnerabilities in web application
Tools needed:
•	OWASP ZAP
OWASP Zed Attack Proxy, is an easy to use integrated penetration testing tools for finding vulnerabilities in web applications while you are developing or testing it.
•	WebGoat
WebGoat is a deliberate insecure application that allows interested developer just like me to test vulnerabilities commonly found in java based applications that use common and open source.
Method and work done:
Setting up work environment on kali Linux for OWASP ZAP and WebGoat.
OWASP ZAP installation
•	Go to browser on your machine and search for OWASP ZAP and download for Linux installer.
•	Go to terminal and change to root user “sudo su”, check your downloaded file in the download directory, using “cd Downloads” and use “ls” to view the directory.
•	Change the file to an executable file “chmod +x “filename””.
•	To lunch the file, (. /”file name”), accept all terms and you’re ready to use ZAP.
Setting up WebGoat
•	Go to browser on your machine and search OWASP WebGoat and go to downloads, you will see standalone jar, click on it and it will redirect you to a Github download page.
•	After downloading the JAR file go to your terminal and change to downloads directory using “cd Downloads”.
•	Check if you have java installed on your machine, (java -- version).
•	To lunch it, type this on the terminal (java jar “file name downloaded”).
•	WebGoat will be lunched and you will see your WebGoat is hosted then you can copy URL address and open on your browser.
Work done:
Scanning WebGoat with OWSAP ZAP 
•	I scanned WebGoat copying the home page url and input it on the space provided by the ZAP for scanning  
•	I entered attack, then it started scanning from 0 to 100%
•	After scanning, there I a bar below that shows the vulnerabilities in WebGoat in order from most critical to less critical.
•	SQL injection is the most critical which occur in the login form.
Image illustration of each steps above.

Scanning process
 

Result after scanning
 
SQL injection with high vulnerability and can be exploited via SQL payloads and the payloads in the red box in the diagram
 
•	I used the manual scan to lunch the WebGoat, and navigate down to injection and down to SQl injection advance and I attempted the task and was able to login to login. Using the SQL UNION SELECT query.
•	Task here, retrieve all data from the table. ‘UNION SELECT userid, user_name, password, cookie, null as f1, null as f2, null as f3 FROM user_system_data;--
•	List of all user data with password is displayed and the I used one of the password to check the password space (passWorD)
 

Next step here after entering the SQL query, got the list of user on it.
 
I used one of password above to check the password, it says congratulation and I was able to access it.
 
 
Challenges faced during task 2
•	Setting up WebGoat on my machine
•	Setting up ZAP on my machine
•	Exploitation of SQL injections
•	Scanning WebGoat with ZAP which took a lot of time 
Solutions to the challenges I faced
•	I made used of materials from Google, Github and YouTube from different instructors.
•	Free up space on my laptop so my kali Linux can function so fast
•	Learnt more about SQL query and payloads.
Conclusion
During the process of my internship with THE RED USERS, I was able to learn more about web application security, how to scan web application using OWSAP ZAP, how to scan for vulnerabilities on wed applications and how to exploit SQL injection on any web application that’s vulnerable to SQL injection.
It’s really great to add more to my knowledge during the internship and also help to keep my hands on desk.
