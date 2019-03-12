# Data Warehouse Data Dictionary
__Final Project__


## Attribute Information
| Course Meetings |Table of Appearence | Contents | Data Type |
|-----------------|---------------------|----------|----------|
|**CRN**|COURSEFACTS|Course Requisite Number...a unique course identifier| Integer|
|**Location**|LOCATION| Identifies the classroom | Text |
|**Day**|Course Meetings|Notes the day of the week | Text|
|**Start**|Course Meetings| identifies date and start time for each class |Text|
|**End**|Course Meetings| Identifies data and end time for each class | Text |
|**CATALOG_ID**|COURSEFACTS| Non unique course identifier | Integer | Text |
|**Section**|Courses| Denotes the section if class if broken up due to size |
|**Credits**|COURSEFACTS| Amount of credits recieved for taking class |
|**Title**|Courses| Course Name|
|**Meetings**|Courses| Contains the day, time and location for the class|
|**Time Codes**|Courses| COntains day time and location|
|**Primary Instructor**|INSTRUCTORS |Teacher name|
|**Cap**|COURSEFACTS|Amount of seats class can have|
|**Act**|COURSEFACTS|Actual amount of seats in occupied in class|
|**Rem**|COURSEFACTS|Remaining seats not taken in a class|
|**Program_Code**|PROGRAM| Class subject identifier|
|**Programs_Name**|PROGRAM|Subject name |
|**Course_Title**|PROGRAM| Class name |
|**Preqs**|COURSE_DIM| Class need before taking this class |
|**Coreqs**|COURSE_DIM| Classes that are needed along with this class |
|**Fees**|Course Catalogs| Price for class |
|**Attributes**|Course Catalogs| Defines what class satisfies |
|**Description**|COURSE_DIM| Summary of the class |
|**term**|COURSEFACTS|Spring - Summer - Winter - Fall|
|**TID**|COURSEFACTS|Professor id number|Integer|
|**CDID**|COURSEFACTS|Course id number|Integer|



