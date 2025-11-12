# H3 Cyberlab

# X) I have summarize few points from given link as below
- Karvinen 2020: Command Line Basics Revisited (https://terokarvinen.com/2020/command-line-basics-revisited/)
  1. Key Navigation Commands: To display the current directory, use the command pwd; to list files, use the command ls; and to change directories, use the command cd.  **less** is used to view files, and piping output to **less** facilitates the management of lengthy outputs.
     
  2. File and Directory Management: Users can make new files and directories with the commands "mkdir," "mv," "cp," and "rm," "rmdir," and "mv."  Simple text editing with keyboard shortcuts is possible with editors such as **nano** and **pico.**

  3. File Transfer and Remote Access: File transfers are made possible by **scp**, while secure remote shell access is made possible by ssh.   During syntax, the target path, server, and user are all supplied. 

  4. Software Installation and System Management: Using package management with **apt-get**, users can install, update, and remove software.   Commands like **man** and **--help **provide documentation, while tab completion and command history boost productivity.
    
- Karvinen 2022: Cracking Passwords with Hashcat (https://terokarvinen.com/2022/cracking-passwords-with-hashcat/)

  1. Fundamentals of Hashes: Systems store passwords as one-way encrypted strings called hashes.   In an attempt to crack them, a computer called Hashcat compares these to dictionary words. 
  2. Instruments and Configuration:   The Debian 11 instruction includes installing Hashcat, HashID, and RockYou, a popular password dictionary with over 14 million entries. 
  3. Determining the Hash Type:  HashID helps determine the hash type (like MD5), which is necessary for Hashcat's -m argument to start the cracking process.
  4. Cracking Method: Hashcat makes use of the identified hash and dictionary file.   The hash 6b1628b016dff46e6fa35684be6acc96 is successfully cracked, revealing the password "summer" in the 
     example. 
  5.Ethics and Performance:  Cracking speed can be accelerated via GPU hardware.   The article emphasizes that you should only use hashes that you own or are allowed to test.

# a) Reserve your presentation title in Moodle:
     - I have not reserved because i have some confusion, will ask on class of 12.11.2025 as i was absent on last class

# b) Linux. Install Linux on a virtual machine. Use Debian 13-Trixie
     - Done

# c) Crack. Crack the hash 6b1628b016dff46e6fa35684be6acc96 . Install hashcat and follow the steps in the article to crack the example hash. Karvinen 2022: Cracking Passwords with Hashcat.
     - I installed hashcat and followed all steps bui i got differnet result while cracking the password "Solved: Nosuch file or directory"

