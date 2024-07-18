GMI conducted an online practical CTF training for GMI and UTEM students. I have an opportunity to join this as GMI alumni. This session focuses on Miscellaneous and Cryptography category. Thanks to Mr Farhan as the instructor and hosting the CTFd platform <3 

<h1>Miscellaneous</h1>
<h2>Pikachu</h2>
<i>Description: Pika Pikaa (25 points)</i><br>
<br>🕵🏻‍♀️ I am given a text file called pikapii.txt. Below is the content of the file:<br>
<br><pre>
GMICTF{P1K4C…R3}
pi pi pi pi pi pi pi pi pi pi pika pipi pi pipi pi pi pi pipi pi pi pi pi pi pi pi pipi pi pi pi pi pi pi pi pi pi pi pichu pichu pichu pichu ka chu pipi pipi pipi pi pikachu pi pi pi pi pi pi pikachu ka ka ka ka pikachu ka ka ka ka ka ka pikachu pipi ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pichu pi pi pi pikachu pipi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pichu pi pi pi pi pi pi pi pi pi pi pikachu pichu pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pipi ka ka ka ka ka pikachu pichu pi pi pi pikachu pipi ka ka ka ka ka ka ka ka pikachu pi pi pi pi pi pikachu pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pi pi pi pi pi pi pi pi pi pi pikachu pichu pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pi pi pi pi pi pi pi pi pi pi pikachu pipi pikachu pichu ka ka ka ka ka ka ka ka ka ka ka pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pipi ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pichu pikachu pipi pipi pi pi pikachu
</pre>
<br>🕵🏻‍♀️ Let’s go to Cipher Identifier to identify.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/09fa0605-fbb6-4d70-8bd4-d5fa19f5ecb8"><br>
<br>🕵🏻‍♀️ Use https://www.dcode.fr/pikalang-language to decrypt the message.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/83c6ed79-b511-4148-9053-47609747fde6"><br>

<h2>1337</h2>
<i>Description: [-|_][†3 Remember the flag format? Apply it here.</i><br>
<br>🕵🏻‍♀️ Let’s use https://www.dcode.fr/leet-speak-1337 to decode the message.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/7853367e-5c6d-478b-8320-cdfd5b296240"><br>
<br>🕵🏻‍♀️ The flag should be `GMICTF{ELITE}`<br>

<h2>Membaca Amalan Mulia</h2>
<i>Description: Head to this page, and try playing around with it :3</i><br>
<br>🕵🏻‍♀️ In this challenge, the instructor himself already showed how to get the flag during the class. But I will interpret in my own understanding. This is what you’ll see when you click on the link.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/dce0e7f0-226b-47e7-808b-d9d7f8c71a5c"><br>
<br>🕵🏻‍♀️ This is what you’ll see when you go to the link and choose number 5. It says I need to check the Javascript.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/32c3694e-42e8-4ff4-8d87-1a5f93166c2a"><br>
<br>🕵🏻‍♀️ From the source page, there’s another file called meep.js. .js extension is a javascript file mentioned in the previous photo. Let’s click on the link.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/186912cc-4183-409b-9a0a-74206c0cbf6d"><br>
<br>🕵🏻‍♀️ Here’s the crucial part. There are 2 functions here; submitNumbers() and callPhpApi(numbers). The submitNumbers() function find checked checkboxes and map values to a string. The callPhpApi(numbers) function uses the fetch API to send a GET request to the PHP script named phr0ng.php. We could use this PHP script to get number 6. <br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/fa4450b2-3361-46cd-8b96-5780043d5560"><br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/9d9fce62-bf55-4ae5-ae38-b0707a22d93a"><br>

<h2>Cheat Code</h2>
<i>Description: Description: Use the cheat code when needed. This is a basic cheat used by alot of nintendo games. After you've pressed the sequence tap on ENTER on your keyboard.</i><br>
<br>🕵🏻‍♀️ This is what you’ll see when you go to the link.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/2c9f7111-987c-4c49-ad1c-ada2af07d3d2"><br>
<br>🕵🏻‍♀️ The hint can be found from the website link itself. This is what I found from Google search.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/0d7903f2-d7eb-4eca-8601-13d504402534"><br>
<br>🕵🏻‍♀️ Try click on your keyboard; up, up, down, down, left, right, left, right, B, A and ENTER. The flag will appear on top on the webpage.<br>
<br><img width="350" alt="image" src="https://github.com/user-attachments/assets/decb5306-c0e7-4483-a0ed-2cd0c28aa22c"><br>

<h1>Cryptography</h1>












