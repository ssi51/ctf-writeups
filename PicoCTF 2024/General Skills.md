1. Super SSH
Description: Using a Secure Shell (SSH) is going to be pretty important. Can you ssh as ctf-player to titan.picoctf.net at port 59228 to get the flag? You'll also need the password 6abf4a82. If asked, accept the fingerprint with yes.

You can use the command ssh ctf-player@titan.picoctf.net -p 59228 to get into the server.
![Screenshot 2024-04-07 181438](https://github.com/ssi51/ctf-writeups/assets/141008956/b1b337e7-f853-44d7-ace6-f789b6296b46)

Flag: picoCTF{s3cur3_c0nn3ct10n_65a7a106}

2. Time Machine
Description: What was I last working on? I remember writing a note to help me remember...
Download the challenge file here: https://artifacts.picoctf.net/c_titan/161/challenge.zip

When I unzip the file, I came across to a came-in directory. When I cat the text file inside the directory, it says "This is what I was working on, but I'd need to look at my commit history to know why..."
![Screenshot 2024-04-07 183116](https://github.com/ssi51/ctf-writeups/assets/141008956/7a379589-4e0e-45ee-8650-69085e256dd3)
When I see "commit history", I'd think of Github and Logs. So, I use the git log command and got the flag instantly.
![Screenshot 2024-04-07 183037](https://github.com/ssi51/ctf-writeups/assets/141008956/0ab66692-19ab-45ac-af5b-a03a543ebdd8)
You may read more about this on https://primer.picoctf.org/#_git_version_control

Flag: picoCTF{t1m3m@ch1n3_8defe16a}
