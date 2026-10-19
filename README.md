# PROG5121POE


PART 1: REGISTRATION AND LOGIN

FEAUTERS

- Username	validation	–	must	contain	an	underscore	( _ )	and	be	no	more	than	5	characters
long.

-Password	complexity	validation	–	must	be	at	least	8	characters	long	and	contain	a	capital
letter,	a	number,	and	a	special	character.

-Cell	phone	number	validation	–	must	contain	the	South	African	international	country	code
(+27)	followed	by	the	number,	correctly	formatted.

-User	registration	–	captures	and	stores	a	user’s	details	once	all	validation	checks	pass,	with
clear	feedback	messages	when	they	don’t.

-Login	–	verifies	that	the	entered	username	and	password	match	the	details	captured	during
registration,	and	returns	an	appropriate	welcome	or	error	message.

-Unit	tests	–	JUnit	tests	covering	all	validation	rules	and	the	registration/login	flow,	using	the
exact	test	data	specified	in	the	assignment	brief.



PROJECT STRUCTURE

-RegistrationApp/

- registration/
-Login.java							
-Main.java
- Core	class:	validation,	registration,	login	logic
- Console	application	entry	point
- LoginTest.java			
- JUnit	test	classs


TECHNOLOGIES USED 

- Java	(developed	and	tested	in	NetBeans	IDE)
- JUnit	4	for	unit	testing


HOW TO RUN TESTS

-NetBeans
Right-click	
LoginTest.java	and	select	Test	File	(or	press	
Alt+F6 )


PART 2: SENDING MESSAGES 


WHAT WAS ADDED 

- Users	can	only	send	messages	after	logging	in	successfully	from part 1.
- The	app	shows	the	welcome	message	“Welcome	to	QuickChat.ˮ
- The	user	picks	from these options in the	menu:
1.	Send	Messages
2.	Show	recently	sent	messages	(displays	“Coming	Soon.ˮ,	still	in	development)
3.	Quit
   
- The	app	keeps	running	until	the	user	chooses	Quit.
- The	user	first	says	how	many	messages	they	want	to	enter,	and	the	app	only	accepts	that	many.
  
- Each	message	records:
1.a	Message	ID:	a	randomly	generated	ten-digit	number
2.the	message	number:	starts	at	0	and	increases	as	messages	are	created
3.the	recipient	cell	number:	must	contain	the	+27	interna1.tional	code
4.the	message	text:	no	more	than	250	characters

- After	writing	a	message	the	user	chooses	to	Send,	Disregard	or	Store	it.
- Stored	messages	are	written	to	a	JSON	file	(storedMessages.json )	so	they	can	be	sent	later.
- When	a	message	is	sent,	its	full	details	are	shown	in	this	order:	Message	ID,	Message	Hash,	Recipient,	Message.
- The	total	number	of	messages	sent	is	shown	when	the	user	quits.


PROJECT STRUCTURE

- Login/
- main/java/com/mycompany/login/
- Login.java										
- Message.java								
- Main.java											
- test/java/com/mycompany/login/
- LoginTest.java						
- MessageTest.java		


TECHNOLOGIES USED 

- Java
- Apache	Maven
- NetBeans	IDE
- JUnit	4	for	unit	testing

HOW TO RUN

In	NetBeans

1.	In	the	Projects	panel,	open	Source	Packages	>	com.mycompany.login .
   
2.	Right-click	QuickChatApp.java	and	choose	Run	File.	This	runs	the	full	application:	registration,	login,	then	the
QuickChat	menu


RUNNING THE TESTS

- In	NetBeans,	right-click	LoginTest.java	or	MessageTest.java	and	choose	Test	File,	or	right-click	the	project	and
choose	Test	to	run	everything.










