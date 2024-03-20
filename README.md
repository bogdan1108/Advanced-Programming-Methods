# Advanced-Programming-Methods

Laboratory 1  
  
1. Provide solutions for the following problems:  
a) Write a Java program that prints the prime numbers among the integers numbers given as command-line parameters.  
b) Write a Java program that prints the maximum value from all the double numbers given as command-line parameters.  
c) Write a Java program that prints the greatest common divisor of all integer numbers given as command-line parameters.  
2. Choose one of the problems below and provide a layered architecture solution (in Java). Requirements necessary for the next lab:  
- Create the classes necessary for just one entity in the problem requirement (the first mentioned entity).  
- The layers should be: domain, repository, service, UI. Use Java packages.  
- Add at least 5 entities in your memory repository (from source code).  
- All entities should be identifiable (use a generic superclass/interface Identifiable) and unique.  
- The UI must allow CRUD operations for the used entity.  
  
a) Design and implement a Java solution for managing the appointments to a dentist. The program should allow CRUD operations for patients, adding a new appointment, cancelling an   appointment, creating different reports, etc.  


Laboratory 2

For your chosen problem implement the requirements below:  
- All entities should be identifiable (use a superclass/interface Identifiable) and unique.  
- Provide a generic interface for the repository and an implementation for a generic memory repository which stores identifiable objects in a Map (HashMap, TreeMap), where the objects identifiers are the keys and the values are the actual objects.  
- Add basic data validation and use the exception mechanism in Java for exceptional situations. Show messages in case of such situations.  
- The UI must allow CRUD operations for both entities.


Laboratory 3  
  
Continue designing and implementing the problem you have chosen. For the next lab you must:  
  
- Implement classes in the repository that allow storing and retrieving data in two formats: text files and binary files (using the Java serialization mechanism). The program must work identically using text and binary file repositories. The decision of which repositories are employed, as well as the location of the repository input files will be made available via the program’s settings.properties file and the Java Properties class. See an example of this file below:  
Repository = binary  
Patients = “patients.bin”  
Appointments = “appointments.bin”  
- Provide tests using JUnit. The test coverage for at least one entity (throughout all layers except UI) must be more than 95%.  


Laboratory 4  
  
Continue the implementation of the problem you have chosen for home assignment 2. For the next lab you must:  
  
- Implement classes in the repository that allow storing and retrieving data to/from a relational database. The decision of which repositories are employed, as well as the location of the repository input files / database will be made available via the program’s settings.properties file and the Java Properties class. See an example is below:  
Repository = database  
Location = data  
Patients = patients  
Appointments = appointments  
Provide various reports, using Java 8 streams. You should create at least 5 different reports. See some examples below:  
  
o all the appointments for a certain patient (and their status);  
o the problems of a certain patient;  
o the phone number of a certain patient (given by id);  
