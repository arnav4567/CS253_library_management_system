# CS253 : Library management system

The assignment implements a library management system in C++ using object oriented programming paradigms. The zip file consists of 4 files - `main.cpp`, and 3 csv files which act as databases:

+ `all_users_data.csv` stores [name,id,password,type of user]. The type of user '1' is for student, '2' is for professor and '3' is for librarian. One row stores details of one user.
+ `all_books_data.csv` stores the details of all books in the library. This file stores the attributes [name of book,author,publisher,isbn code, is_issued]. The `is_issued` field is 1 if the book has been issued by a user and zero otherwise. One row in the file stores the data of one book.
+ `issued_books_data` stores [user id,name of book,isbn code, timestamp]. The user id is the id of the user who issued the book and `timestamp` stores the time when the user issued it. The timestamp will help us later in calculating the fine for users.

To run the system, type the following commands in the console:
``` 
g++ main.cpp -o main
.\main
```
The system will run on the console. <br>
<br>
NOTE: A default librarian exists in the csv files with the following creadentials:
+ [libname,libraryid,1234,3]. This user should not be deleted.