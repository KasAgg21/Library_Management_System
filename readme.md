Library Management System

![68747470733a2f2f692e696d6775722e636f6d2f63304e566272792e706e67](https://user-images.githubusercontent.com/73023696/234069491-2688c392-6bfd-440b-84c5-38a52f1489bf.png)

Normalization
CARD (Number, Fines, Status)
CUSTOMER (ID, Name, Address, Phone_number, Card_number [References CARD(Number)], Password, User_name, Date_sign_up)
EMPLOYEE (ID, Name, Address, Phone_number, Card_number [References CARD(Number)], Password, User_name, Paycheck, Branch_name [References BRANCH(Name)])
BRANCH (Name, Address [References LOCATION(Address)], Phone_number)
LOCATION (Address)
RENT (Card_ID [References CARD(Number)], Item_ID [References BOOK or VIDEO(ID)], Date, Return_date)
BOOK (ISBN, ID, State, Avalability, Deby_cost, Lost_cost, Address [References LOCATION(Address)])
VIDEO (Title, Year, ID, State, Avalability, Deby_cost, Lost_cost, Address [References LOCATION(Address)])
