# Data Warehouse Data Dictionary
__Final Project__


## Attribute Information
| Course Meetings |Table of Appearence | Contents | Data Type |
|-----------------|---------------------|----------|----------|
|**CRN**|COURSEFACTS|Course Requisite Number...a unique course identifier| Integer|
|**Location**|LOCATION| Identifies the classroom | Text |
|**CATALOG_ID**|COURSEFACTS| Non unique course identifier | Integer | Text |
|**Credits**|COURSEFACTS| Amount of credits recieved for taking class |
|**Primary Instructor**|INSTRUCTORS |Teacher name|
|**Cap**|COURSEFACTS|Amount of seats class can have|
|**Act**|COURSEFACTS|Actual amount of seats in occupied in class|
|**Rem**|COURSEFACTS|Remaining seats not taken in a class|
|**Program_Code**|PROGRAM| Class subject identifier|
|**Programs_Name**|PROGRAM|Subject name |
|**Course_Title**|PROGRAM| Class name |
|**Preqs**|COURSE_DIM| Class need before taking this class |
|**Coreqs**|COURSE_DIM| Classes that are needed along with this class |
|**Description**|COURSE_DIM| Summary of the class |
|**term**|COURSEFACTS|Spring - Summer - Winter - Fall|
|**TID**|COURSEFACTS|Professor id number|Integer|
|**CDID**|COURSEFACTS|Course id number|Integer|



