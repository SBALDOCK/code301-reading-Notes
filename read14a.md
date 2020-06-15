### Database Normalization Explained in Simple English

* **Database Normalization** is a process used to organize a database into tables and columns
* Tables should be about a specific topic and only supporting topics included
* Reducing the table to a single purpose reduced the number of duplicate data contained within the database
* Eliminates issues steming from database modifications


* Three normal forms most databases adhere to using
  * As tables satisfy forms, they are less prone tio modification anomalies and more focused toward a sole purpose or topic

* Three reasons to normalize a database
  * Minimize duplicate data 
    * Increases storage and decreases performance
    * Becomes difficult to maintain data changes
  * Minimize or avoide data modificiation issues
    * Insert Anomaly, update anomaly, deletion anomaly
  * Simplify queries
    * Much easier to search and sort for data

* Three common forms of database normalization
  * **First Normal Form** - the information is stored in a relational table with each column containing atomic values. No repeating groups of columns
  * **Second Normal Form** - Tables is in first normal form and all columns depend on the table's primary key
  * **Third Normal Form** - Table is in second normal form and all columns are not transitively dependent on the primary key
