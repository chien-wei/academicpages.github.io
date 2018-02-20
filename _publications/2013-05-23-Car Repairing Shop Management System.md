---
title: "Car Repairing Shop Management System"
collection: publications
permalink: /projects/garage
excerpt: 'My first project of object-oriented C++ and using Visual Studio unit testing.'
date: 2013-05-23
---

My first project of object-oriented C++ and using Visual Studio 2012 unit testing.

## Abstract
Generally, when customers drive into the repairing depot, or the car is towed into the repairing depot, a senior technician quickly help you assess what needs to be done or what items are needed for maintenance, and then is currently waiting for maintenance of vehicles, available equipment status, and the number of technicians working today to give you an estimated completion time and the initial offer, due to the current material control and logistics systems are developed, so a variety of car models of various repair parts have been established computer System, you can check the price of the required materials, garage for a variety of models of the fault conditions and maintenance procedures are also in the computer to establish a standard process, so technicians simply type the basic customer vehicle information, select the maintenance of the project, the program You can automatically figure out the estimated time to take the car and the initial offer, the job is to try to establish such a system.  

## Data

| Material ID | Material Name    | Price | Need Bumper | Warranty(Month) |
|-------------|------------------|-------|-------------|-----------------|
| a24         | Headlight bulb   | 2000  | 0           | 12              |
| a25         | Front lamp cover | 600   | 0           | 12              |
| a26         | Air filter       | 1200  | 0           | 12              |
| a31f        | Front door lock  | 2600  | 0           | 24              |
| ...         |                  |       |             |                 |
| c01         | Wheels           | 2200  | 1           | 6               |
| ...         |                  |       |             |                 |

| Repair ID | Materials needed | Repair times |
|-----------|------------------|--------------|
| 1001      | a31f, a32, b01   | 20           |
| ...       |                  |              |
| 2001      | c01, c02, d02    | 60           |
| ...       |                  |              |



## Result
```
Enter today's date: (year, month, day) 2013 5 1

[S]tatus update/[N]ew request? S
Current time? (hour, minute) 9 0

There is no car currently being maintained!

[S]tatus update/[N]ew request? N
Service request time: (hour, minute) 9 20 
License Plate: 8934-NX 
Number of Service Items: 2 
Service Items: 1002 1004
Expected finish time: 2013/05/01 10:44

[S]tatus update/[N]ew request? S
Current time? (hour, minute) 9 30

[0000] 8934-NX, Time requested:  2013/05/01 09:20 ,
                Service requested: 1002, 1004,
                Service started on 2013/05/01 09:20 ,
                Charge=NT7900
   ===> Expected finish time:  2013/05/01 10:44

[S]tatus update/[N]ew request? N
Service request time: (hour, minute) 9 50
License Plate:  1234-AB 
Number of Service Items: 2 
Service Items: 1003 2001
Expected finish time: 2013/05/01 12:30

[S]tatus update/[N]ew request? S
Current time? (hour, minute) 10 10

[0000] 8934-NX, Time requested:  2013/05/01 09:20 ,
                Service requested: 1002, 1004,
                Service started on 2013/05/01 09:20 ,
                Charge=NT7900
   ===> Expected finish time:  2013/05/01 10:44
[0001] 1234-AB, Time requested:  2013/05/01 09:50 ,
                Service requested: 1003, 2001,
                Service not yet started.,
                Charge=NT15600
   ===> Expected finish time:  2013/05/01 12:30

[S]tatus update/[N]ew request? N
Service request time: (hour, minute) 17 20 
License Plate: 4444-RR 
Number of Service Items: 2 
Service Items: 2003 2004
Expected finish time: 2013/05/01 19:14
Sorry, it's too late to accept this request!

[S]tatus update/[N]ew request? S
Current time? (hour, minute) 17 30

[0000] 8934-NX, Time requested:  2013/05/01 09:20 ,
                Service requested: 1002, 1004,
                Service started on 2013/05/01 09:20 ,
                Service finished on 2013/05/01 10:39 ,
                Charge=NT7900
[0001] 1234-AB, Time requested:  2013/05/01 09:50 ,
                Service requested: 1003, 2001,
                Service started on 2013/05/01 10:49 ,
                Service finished on 2013/05/01 12:20 ,
                Charge=NT15600
There is no car currently being maintained!

[S]tatus update/[N]ew request? N
Service request time: (hour, minute) 17 31
```