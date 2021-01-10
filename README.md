# Module 2 Capstone - TEnmo

Java console program that implements SQL and Spring Boot which allows funds transfers from one user to another. 

## Features

1. User is able to register with a username and password.
   1. A new registered user starts with an initial balance of 1,000 TE Bucks.
2. User is able to log in using registered username and password.
   1. Logging in returns an Authentication Token which is required for all subsequent interactions with system outside of registering and logging in.
3. An authenticated user is able to see Account Balance.
4. An authenticated user is able to *send* a transfer of a specific amount of TE Bucks to a registered user.
   1. User is able to choose from a list of users to send TE Bucks to.
   2. A transfer includes the User IDs of the from and to users and the amount of TE Bucks.
   3. The receiver's account balance is increased by the amount of the transfer.
   4. The sender's account balance is decreased by the amount of the transfer.
   5. User cannot send more TE Bucks than they have in account.
   6. A Sending Transfer has an initial status of "approve."
5. An authenticated user is able to see transfers they have sent or received.
6. An authenticated user is able to retrieve the details of any transfer based upon the transfer ID.


## Screen Layouts

### Current balance
```
Your current account balance is: $9999.99
```

### Send TE Bucks
```
-------------------------------------------
Users
ID          Name
-------------------------------------------
313         Bernice
54          Larry
---------

Enter ID of user you are sending to (0 to cancel):
Enter amount:
```

### View transfers
```
-------------------------------------------
Transfers
ID          From/To                 Amount
-------------------------------------------
23          From: Bernice          $ 903.14
79          To:    Larry           $  12.55
---------
Please enter transfer ID to view details (0 to cancel): "
```

### Transfer details
```
--------------------------------------------
Transfer Details
--------------------------------------------
 Id: 23
 From: Bernice
 To: Me Myselfandi
 Type: Send
 Status: Approved
 Amount: $903.14
```
