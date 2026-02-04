SRSAdmin 2.0 Final
SRSAbbo 1.0

noBSoft (c) 2003


Installation
jvm
installing
troubleshooting
SRSAbbo
creating accounts
account menu
warnings
SRSAdmin
configuration
operation
maintainance
statistics


Installation

Java Virtual Machine
This software is made in java so a virtual machine is needed to run them.
The setup file for JDK v1.4 can be found in the root directory of your installation cd.
The default setup settings should work fine.

Installing the program(s)
This software creates a database file in the directory from which it was started.
On the installation cd are two separate subdirectories containing the program files of each program.
Copy the directory and its entire contents, of the program you wish to install to your hard drive.
Both directories contain a ".BAT" which can be used to start up the programs.
If you see something like "starting up, database saved!" open your browser to http://localhost to connect.

Trouble-shooting
--Both programs are webservers that claim port 80 on every interface so you can't run them on the same computer at the same time.
You'll get something like "server socket bind exception, address already in use"
--CLASSPATH is an environment setting which needs to be set to the directory or .jar file containing jdk libraries.
If you're not starting the VM from the directory containing the program files, make sure it also contains the path there.
--If you are running the browser and server on a separate computers make sure they have proper networking access to eachother.


SRSAbbo
Creating Accounts
Just enter the name of the account you wish to add, at the bottom at the screen.
The resulting screen should be printed out and kept at a safe place at it contains the I.D. to the account.
Account Menu
Once logged in the amount of credits in an account can be increased and decreased.
The resulting screens show a summary of the account details and the last 10 mutations made to it.
The remove account button does not prompt for confirmation so don't click on it unless you want to.
Warnings
The mainmenu will request human intervention for accounts which have not been accessed for at least 30 days or have negative credit by signaling red texts.

SRSAdmin

Configuration
--The default passwords for user- and administrator-login are "user" and "ramzi".
These can be changed by clicking on the "passwords" button in the administrator main menu.
--Before you can offer your products lists need to be made of their names and prices.
These lists are divided by groups which can be made by clicking on the "add group" button at the bottom of the group list in the main menu.
A new button with the name of the group you entered will appear.
To add produkts to a group you must enter the group by clicking on its button in the main menu.
Produkts are created in the same way as groups: just click on "add produkt".
To set the prices of the new produkt you must view the produkt by clicking on its button in the group menu.
In this screen you can also change the amount remaining to be warned for low inventory.
--Make sure you have set the proper in-prices of all your products before you continue to enter your inventory!
In the group menu click on the inventory button for an overview of current inventory and it's value.
Here you can add produkts to your inventory.
To remove items your inventory you can not only sell them but also enter the view product screen and click on "remove inventory".

Operation
--To sell products you need to enter the user password and press the appropriate button in the log-in screen.
First select a group then a produkt. Enter the amount of items of this type to be sold.
A section will appear whcih shows the items to be sold and allows them to be removed
To add more produkts to this transaktion choose a group then a produkt in the same way as before.
Optionally enter an amount of discount then click on "make receipt" to finalize the transaction.
The result screen can be printed as receipt for the customer.
Clicking on the buttom at the bottom saves the transaction.
--Flexphone stats should be entered daily. Enter the low number in the "spent" box and the high number in the "earned" box.

Maintainance
--You can add items to the inventory whenever you want but make sure the in-price of the product-type has been updated first.
--To use the credit system uncheck the "paid" checkbox in the screen prior to making a receipt. Enter a descriptive name in the comment field.
For an overview of unpaid transaktions click on the "credit" button at the top of the user menu.
--A transaktion can be completely undone by entering the receipt number (printed on the receipt) is entered into the "undo sale" box in the administrator menu.
The original in-price of the produkts is maintained.

Statistics
--The date thing in the administrator menu runs van 0:00 to 0:00 so to view the statistics of the whole day of 20/02/03, select from 20/02/03 to 21/02/03.
--Clicking on the name of a group shows a list of product sales.
--Clicking on the name of a produkt shows a list of transaktions in which it was sold.
--Clicking on the date of a transaktion shows a summary of the transaktion and it's product(s).

DEFAULT LANGUAGE TEXTS:
01SELECT LOGIN
02USER
03ADMINISTRATOR
04CASH
05PLASTIC
06LOGOFF
07SET
&#8364;
09YOU HAVE LOGGED IN
10USER NOT FOUND!
11INCORRECT PASSWORD!
12ITEM(S) ADDED
13CODE NOT FOUND!
14ITEM(S) REMOVED
15RECEIPT SAVED
16YOU ARE NOT LOGGED IN
17CASH SET
18PLASTIC SET
19DATABASE CLEARED
20FROM
21TO
22ADMIN PASSWORD SET
23<font color=green>USER ADDED</font>
24<font color=red>USER REMOVED</font>
25BACK TO GROUP STATS
26BACK TO TYPES
27BACK TO MAIN
28PLEASE CLOSE THIS WINDOW
29GROUPS
30NEW GROUP
31ADD GROUP
32STATISTICS
33CLEAR DATABASE
34LOGIN HISTORY
35PASSWORDS
36UNDO SALE
37PURCHASE
38SHUT DOWN
39GROUP CREATED
40GROUP REMOVED
41<font color=red>GROUP NAME ALREADY EXISTS!</font>
42INVENTORY
43REMOVE GROUP
44NEW TYPE
45ADD TYPE
46BACK TO GROUPS
47TYPE CREATED
48TYPE REMOVED
49<font color=red>TYPE NAME ALREADY EXISTS!</font>
50REMOVE INVENTORY
51REMOVE TYPE
52NAME
53CODE
54IN-PRICE
55OUT-PRICE
56MINIMUM
57SAVE TYPE
58TYPE SAVED
59ITEMS REMOVED!
60TYPE
61#INVENTORY
62VALUE
63ADD
64TOTAL
65ADD TO INVENTORY
66INVENTORY ADDED
67LOW INVENTORY
68EXISTING USERS
69NONE
70ADD USER
71USER NAME
72NEW USER
73ADMIN PASSWORD
74SAVE PASSWORD
75DELETE
76SCAN
77FLEXPHONE
78SPENT
79EARNED
80SEPARATE SALE
81DESCRIPTION
82SAVE
83FLEXPHONE SAVED
84SALE COMPLETED
85ITEMS
86REMOVE
87PRICE
88DISCOUNT
89PAYMENT
90COMMENT
91MAKE RECEIPT
92PRODUCT
93AMOUNT
94BTW 19%
95NUMBER
96SOLD BY
97DATE
98THANK YOU FOR YOUR PURCHASE
99PURCHASE ADDED
100SALE UNDONE
101RECEIPT NUMBER NOT FOUND!
102ALL ACCOUNTS
103FILTER
104FOR
105SALES STATISTICS FOR
106SOLD
107PROFIT
108TURNOVER
109GROUP
110PURCHASE STATISTICS
111BOUGHT
112BACK TO STATISTICS
113BACK TO TYPE STATS
%EOF%
%EOF%
%EOF%
%EOF%
%EOF%
%EOF%