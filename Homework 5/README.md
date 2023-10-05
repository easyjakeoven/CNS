## Homework 5
1/c Jake Carpenter, CNS, 05OCT23


## Part 2

Step 6 of 10.2:
![Screenshot 1](step6_of_10.2.png)


Step 12 of 10.2:
![Screenshot 1](step12_of_10.2.png)


Step 4 of 10.4:
![Screenshot 1](step4_of_10.4.png)


Step 9 of 10.4:
![Screenshot 1](step9_of_10.4.png)


## Part 3

![Screenshot 1](part3_1.png)
I downloaded a linux virtual box to do the assignment in. I generated my SSH keys in it before I SSHed into my Jump Box.




![Screenshot 1](part3_2.png)
I copied my public key into my Jump Box from my VM.




![Screenshot 1](part3_3.png)
I was able to log into my Jump Box without having to type in my password.





## Part 4

![Screenshot 1](part4_1.png)
I changed my password on my Jump Box to a password in the top 100 (123456).




![Screenshot 1](part4_2.png)
I installed Hydra on my VM and ran the program. I attempted to download the reccommended text file, but I was having a bunch of issues getting Hydra to run with it. So I created a new text file titled "worst_passwords.txt," copied all the passwords in the original list, and ran that in Hydra instead.




![Screenshot 1](part4_3.png)
I successfully brute-forced the password.
