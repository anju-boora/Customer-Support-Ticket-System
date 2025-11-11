# Customer-Support-Ticket-System
Problem: Develop the Customer Support Ticket System 
Description: The Customer Support Ticket System is a software solution designed to manage incoming customer tickets using queues, stacks, and linked lists. This system enables dynamic addition of tickets, prioritizes urgent tickets, supports undo operations, and processes tickets in a round-robin manner. The lab assignment focuses on implementing these data structures in C++ or Python to address real-world customer support scenarios and analyzing their functionality. 
Implementation Sub-Problems 
1.	Create a singly linked list for dynamically adding tickets to the system.  
2.	Use a stack for undo operations (e.g., remove last inserted ticket).  
3.	Implement a priority queue to process urgent tickets first.  
4.	Demonstrate circular queue for round-robin ticket processing.  
5.	Represent billing history using polynomial linked lists for record comparison. 
Evaluation Metrics 
Metric 	Marks Excellent Very Good Satisfactory Poor 
Problem Understanding 	2 	2 	1.5 	1 	0.5 
Problem Solving Approach 	2 	2 	1.5 	1 	0.5 
Completion of the Problem 	2 	2 	1.5 	1 	0.5 
Participation during Class/Lab 	2 	2 	1.5 	1 	0.5 
Explanation of the Assignment 	1 	1 	0.75 	0.5 	0.25 
Attendance 	1 	1 	0.75 	0.5 	0.25 
Assignment Objectives 
a.	Develop a foundational understanding of C++ and Python programming and linear data structures (linked lists, stacks, queues). 
b.	Gain practical experience with singly linked lists, stacks, priority queues, and circular queues. 
c.	Implement real-world applications for customer support ticket management. 
d.	Understand the application of stacks and queues in undo operations and priority-based systems. 
e.	Apply polynomial linked lists for record comparison in billing history. 
Assignment Instructions 
1. Ticket ADT Design 
Attributes: 
a.	TicketID: Integer, unique identifier for the ticket. 
b.	CustomerName: String, name of the customer. 
c.	IssueDescription: String, details of the customer’s issue. 
d.	Priority: Integer, priority level of the ticket (e.g., 1 for urgent).  
Methods: 
a.	insertTicket(data): Insert a new ticket record into the singly linked list. 
b.	deleteTicket(TicketID): Remove a ticket record based on the TicketID. 
c.	retrieveTicket(TicketID): Retrieve ticket details based on the TicketID. 
2. Customer Support Ticket System 
Attributes: 
a.	TicketList: A singly linked list to store ticket records dynamically. 
b.	UndoStack: A stack to store recent ticket changes for undo functionality. 
c.	PriorityQueue: A priority queue to manage urgent tickets. 
d.	CircularQueue: A circular queue for round-robin ticket processing. 
e.	BillingHistory: A polynomial linked list to represent billing records. 
Methods: 
a.	addTicketRecord(): Add a new ticket to the singly linked list and update the undo stack. 
b.	undoTicketOperation(): Revert the most recent ticket operation using the stack. 
c.	processPriorityTickets(): Enqueue and dequeue tickets in the priority queue based on urgency. 
d.	processRoundRobinTickets(): Manage ticket processing using the circular queue. 
e.	compareBillingHistory(): Use polynomial linked lists to compare billing records. 
Implementation Steps 
1.	Define the Ticket ADT with the specified attributes and methods using a singly linked list structure in C++ or Python.  
2.	Implement a stack-based undo mechanism to track and revert ticket operations.  
3.	Develop a priority queue to process urgent tickets first.  
4.	Create a circular queue for round-robin ticket processing.  
5.	Implement polynomial linked lists to represent and compare billing history records. 
Evaluation Criteria 
Criteria 	Marks 	Description 
Problem 
Understanding 	2 	Demonstrates clear understanding of the problem requirements and objectives. 
Problem Solving Approach 	2 	Effective approach to designing and implementing linked lists, stacks, and queues in C++ or Python. 
Completion of the Problem 	2 	Complete implementation of all required components (linked lists, stacks, queues, polynomial operations). 
Participation during Class/Lab 	1 	Active engagement in class/lab discussions and activities related to the lab assignment. 
Explanation of the Assignment 	2 	Clear and detailed explanation of the implemented solution in the submission report. 
Attendance 	1 	Consistent attendance in classes/labs relevant to the lab assignment. 
Prerequisites 
•	Familiarity with pointers and structures in C++ and basic programming in Python.  
•	Basic knowledge of linked list implementation. 
Concepts Covered 
•	Stacks, queues, linked lists, polynomial operations.
code output:Added Ticket: [1] Alice - Cannot login (High)
Added Ticket: [2] Bob - Payment not processed (Normal)
Added Ticket: [3] Charlie - App crash issue (High)

--- All Tickets ---
[1] Alice - Cannot login (High)
[2] Bob - Payment not processed (Normal)
[3] Charlie - App crash issue (High)

--- Processing Queue ---
Current Processing Queue:
[3] Charlie - App crash issue (High)
[1] Alice - Cannot login (High)
[2] Bob - Payment not processed (Normal)
Processing Ticket: [3] Charlie - App crash issue (High)
Undo Process: Re-added [3] Charlie - App crash issue (High) to queue
Processing Ticket: [1] Alice - Cannot login (High)
