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
</pre>

<h1> Binhexa </h1>
<i>Description: How well can you perfom basic binary operations? Additional details will be available after launching your challenge instance.</i><br>
<br> 🕵🏻‍♀️ They will provide a shell to connect with. This is how it'll look like at first:<br>
<br>![Screenshot 2024-05-19 114238](https://github.com/ssi51/ctf-writeups/assets/141008956/4bab50e0-04e4-4d2f-9098-8c8c125708c9)<br>
<br> 🕵🏻‍♀️ These two websites are very helpful to solve this challenge:<br>
<br> - https://www.rapidtables.com/calc/math/binary-calculator.html<br>
<br> - https://bit-calculator.com/bit-shift-calculator<br>
<br>![Screenshot 2024-05-19 120100](https://github.com/ssi51/ctf-writeups/assets/141008956/0e157ef5-bea1-40e5-9f08-1a9dd2aa7c64)

Flag: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d6f8047e}

<h1>Binary Search</h1>
<i>Description: Want to play a game? As you use more of the shell, you might be interested in how they work! Binary search is a classic algorithm used to quickly find an item in a sorted list. Can you find the flag? You'll have 1000 possibilities and only 10 guesses.
Cyber security often has a huge amount of data to look through - from logs, vulnerability reports, and forensics. Practicing the fundamentals manually might help you in the future when you have to write your own tools!
Download the challenge file here: https://artifacts.picoctf.net/c_atlas/5/challenge.zip</i><br>
<br> 🕵🏻‍♀️ I get to solve this by just guessing the number.<br>
<br>![Screenshot 2024-05-19 120524](https://github.com/ssi51/ctf-writeups/assets/141008956/17c4c1b4-6c08-446c-be2a-72d3cbfc830b)
Flag: picoCTF{g00d_gu355_3af33d18}<br>
<br> You can read more on Binary Search. It is the most basic searching algorithm in CS course. This is how what I learn using C++ :
<br> - To use binary search, the data must be in order.
<br> - Binary search starts by testing the data in the element at the middle of the array, to determine if the target is in the first (left) or the second half (right) of the list.
<br> - To find the middle of the list, we need three variables; one to identify the beginning of the list (begin), one to identify the middle of the list (mid) and one to identify the end of the list (end)
<pre>
  Algorithm BinarySearch(array, size, target, locationWanted)
  1. Set begin=0, end=size-1, mid=0;
  2. Set found = false;
  3. While (begin <= end)
    1. mid = (begin + end) / 2;
    2. if (target > array[mid])
      1. begin = mid + 1
    3. else if (target < array[mid])
      1. end = mid - 1;
    4. else
      1. begin = end + 1
      2. found = true;
      3. locationWanted = mid;
  4. Return found
</pre>
