## [Lab-01](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_01/Lab_01.md)
Question: 01
What are the disadvantages of file processing system?

### Answer:
```
Disadvantages of File Processing System:

- Slow access time
Direct access of files is very difficult and one needs to know the entire
hierarchy of folders to get to a specific file. This involves a lot of time.

- Presence of redundant data 
The same data can be present in two or more files which takes up more disc
space.

- Inconsistent Data
Due to data redundancy, same data stored at different places might not match
to each other.

- Data Integrity Problems
The data present in the database should be consistent and correct. To achieve
this, the data should must satisfy certain constraints.

- Difficulty in recovery of corrupt data
Recovery or backup of lost and corrupt data is nearly impossible in case of File
Processing System.

- Lack of Atomicity
Operations performed in the database must be atomic i.e. either the operation
takes place as a whole or does not take place at all.

- Unauthorized Access
Anyone who gets access to the file can read or modify the data.
```