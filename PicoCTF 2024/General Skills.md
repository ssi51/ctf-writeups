<h1> Super SSH </h1> 
<i>Description: Using a Secure Shell (SSH) is going to be pretty important. Can you ssh as ctf-player to titan.picoctf.net at port 59228 to get the flag? You'll also need the password 6abf4a82. If asked, accept the fingerprint with yes. </i><br>

<br> 🕵🏻‍♀️ You can use the command ssh ctf-player@titan.picoctf.net -p 59228 to get into the server.<br>
<br>![Screenshot 2024-04-07 181438](https://github.com/ssi51/ctf-writeups/assets/141008956/b1b337e7-f853-44d7-ace6-f789b6296b46)

Flag: picoCTF{s3cur3_c0nn3ct10n_65a7a106}

<h1> Time Machine </h1>
<i>Description: What was I last working on? I remember writing a note to help me remember...
<br>Download the challenge file here: https://artifacts.picoctf.net/c_titan/161/challenge.zip</i>

<br> 🕵🏻‍♀️ When I unzip the file, I came across to a came-in directory. When I cat the text file inside the directory, it says "This is what I was working on, but I'd need to look at my commit history to know why..."<br>
<br>![Screenshot 2024-04-07 183116](https://github.com/ssi51/ctf-writeups/assets/141008956/7a379589-4e0e-45ee-8650-69085e256dd3)<br>
<br> 🕵🏻‍♀️ When I see "commit history", I'd think of Github and Logs. So, I use the git log command and got the flag instantly.<br>
<br>![Screenshot 2024-04-07 183037](https://github.com/ssi51/ctf-writeups/assets/141008956/0ab66692-19ab-45ac-af5b-a03a543ebdd8)
<br>You may read more about this on https://primer.picoctf.org/#_git_version_control

Flag: picoCTF{t1m3m@ch1n3_8defe16a}

<pre>
ssi51-picoctf@webshell:~/2024$ ls
challenge.zip  drop-in
ssi51-picoctf@webshell:~/2024$ cd drop-in
ssi51-picoctf@webshell:~/2024/drop-in$ ls
message.txt
ssi51-picoctf@webshell:~/2024/drop-in$ cat message.txt
This is what I was working on, but I'd need to look at my commit history to know why...
ssi51-picoctf@webshell:~/2024/drop-in$ git log
</pre>
