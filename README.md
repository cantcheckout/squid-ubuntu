Pre-requisite:

Instructions are for Ubuntu 14 (64bit)

1. Install expect
   $ sudo apt-get update
   $ sudo apt-get install expect
   $ sudu apt-get install git
   $ sudo apt install squid
   
Run the program
1. Launch Terminal
2. Type the command
       $ git clone https://github.com/javonz3/squid-ubuntu
3. Browse the checkout files i.e 
       $ cd squid_ubuntu
4. Run the command
       $ ./script.py   IF USING ADMIN PASSWORD (This may work with or without password)
       $ ./script.py -w     IF WITHOUT SPECIFYING PASSWORD
5. When using OS with ADMINISTRATIVE PASSWORD, 
      supply it and hit enter button to proceed
6. Done

Notes: 
	1 Log.log file will be created name Log.log.
	2. When adding new User and or password, 
	      it should not contain space " " or not empty.
	3. Never move or alter the script.py file or transfer to another folder.
	4. You can transfer the script.py python file together with its folder and its hidden dependency files.


To uninstall squid:
    1. sudo apt-get remove apache2-util squid
    2. sudo apt-get autoremove
    2. sudo rm /etc/squid3/squid.*

How to update existing port number:
	1. At your terminal, browse script folder
		i.e cd ~/Download/squid-ubuntu
	2. ./script -p <PORT NUMBER>
  
The above steps can be done with the single line:

     sudo apt-get update && echo y | sudo apt-get install expect && sudo apt-get install git && git clone https://github.com/liomedal/squid-ubuntu && cd squid-ubuntu && ./script.py
