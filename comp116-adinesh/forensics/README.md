Nate Tenczar: ntencz01

Aswathy Dinesh :adines01

# 				Assignment 5: Forensics

#1

Image A is hiding another image, prado.jpg, which was discovered using
steghide on Image A.

Images B and C are the same, as shown by using cmp.

#2

1. FAT16 and EXT

2. There is no phone carrier involved.

3. Kali GNU/Linux 1.0, found in ext partition at /etc/issue

4. Metasploit is installed in /opt
   Truecrypt is installed (there are config files in /root/.Truecrypt)
   Cowsay and Cowthink are installed in /usr/games
   There are plenty of other binaries located in /bin and /sbin

5. The root password is "toor", which was found using john the ripper on the
   passwd and shadow files (unshadow passwd shadow). Also, the default
   password for Kali linux is "toor".

6. There are no additional user accounts on the system.

7. There is incriminating evidence of the suspect stalking the celebrity
   (Celine Dion) in /root/Documents and /root/Pictures. More evidence was
   found in the restored directory of files from photorec, by running
   grep on the directory of recovered files (grep -r "celine").

8. The suspect removed some pictures (00265065.jpg,05027337.jpg,05028809.jpg,
   05030409.jpg, 05030585.jpg, 05038313.jpg, 05038553.jpg,05038569.jpg,
   05038753.jpg,05039049.jpg,05158537.jpg,06942793.jpg, 05030089.pdf) of Celine
   Dion and a ticket confirmation email pdf that he took to visit celine in Las
   Vegas. This was found by using foremost and photorec file recovering
   programs.

9. There is a truecrypted file .Dropbox.zip under /root. Used truecrack and
   john the ripper wordlist to gain access(password is ‘iloveyou’), and found an
   mp4 file of a celine dion song and a picture of tickets.

10. There is a pdf of an email containing a receipt for a ticket to see
    Celine Dion at Caesar's Palace (Las Vegas, NV) on July 28th, 2012. This was
    found by recovering all the files on the disk using photorec, then searching
    through all the pdfs for "ticket" (using grep -r "ticket")

11. Found a truecrypted file .Dropbox.zip and lots of deleted image and pdf
    files.

12. Celine Dion is the celebrity being stalked (in /root/Documents and
    /root/Pictures there are images and setlists)
