# TireFire
*	TireFire is a scalable and straightforward platform for external enumeration to place your operations and workflow order. 
*	The database for TireFire (Main.csv) is easily altered to support your methodologies as they are substituted and appended.
*	TireFire is a product of 19% security solutions. 
* ReRelease is scheduled for March 6 2021
![alt text](https://github.com/CoolHandSquid/TireFire/blob/TireFire_V3/Images/Tire_fire.jpg)
## Friendly (GUI-ish) Interface
![alt text](https://github.com/CoolHandSquid/TireFire/blob/TireFire_V3/Images/2_kickoff.png)
![alt text](https://github.com/CoolHandSquid/TireFire/blob/TireFire_V3/Images/3_TireFire.png)
## Usage
*	TireFire will not function well if not run as root.
*	Once Build.sh has been run, TireFire will have been added to your path.
*	Type "TireFire 10.10.10.5" and you will be yeeting with a cyber **cannon!**
*	From the "Main Table," type the corresponding number of a protocol for which you would like to run a scan.
*	From the "Protocol Table," click the corresponding number of a scan you would like to run. The scan will be kicked off in another tab.
*	Hit enter to return to the "Main Table."
*	You can change the variables by going to the "Variables Table."
*	If there is a scan or series of scans for a protocol, you would like to add, edit Main.csv following the guidelines in this README (it's pretty straight forward).
*	Tables and commands can be added while TireFire is running, and it will be populated once Main.csv is saved.
## ProTips
- Ctrl+Z will bring you back to the main TireFire Page.
- Ctrl+PageUp/PageDown will allow you to peruse through open tabs.
## How to Build
- git clone https://github.com/CoolHandSquid/TireFire.git
- cd TireFire
- sudo /bin/bash ./Build.sh 
## Easily Add modules
- Open Main.csv with your favorite csv editor (I'm partial to ModernCSV).
- When adding a command, keep in mind Name, Port, and Description are for the primary display screen; Cmd_Name, Cmd_Description, Cmd_Command, Cmd_Comment, and SubDisplayOrder are for the secondary display screen.
## Special Characters and Syntax
-	Cmd_Command has a few special characters including &&&&, #, and {}.
-	&&&& Anywhere in the command will split the line and start each command individually in separate tabs.
  -	Example: whoami &&&& id &&&& ifconfig will open three tabs and run the desired command in each. &&&& is useful if you initially run multiple separate commands every time you see a specific port open.
-	"#" is for sending yourself notes to another tab. Using "#" as a special character will only work if the first character of the first line is #. "#" can be useful if you don't want to run a command, but you want to give yourself copy-paste notes for manual enumeration.
-	{} is for grabbing a variable from TireFire. Available variables are IP, Domain_Name, Naming_Context, Web_Proto, Web_Port, Big_Passwordlist, Small_Passwordlist, Big_Userlist, Small_Userlist, Big_Dirlist, Small_Dirlist.
-	Use " instead of ' due to the way that the string is being passed into TireFire.  

![alt text](https://github.com/CoolHandSquid/TireFire/blob/TireFire_V3/Images/1_csv.png)
![alt text](https://github.com/CoolHandSquid/TireFire/blob/TireFire_V3/Images/CoolHandSquid.jpg)
## Contact
Please contact me at CoolHandSquid32@gmail.com for suggestions and ideas!













