## Database Systems

This assignment involves practical tasks using the MySQL command-line interface to demonstrate understanding of core database concepts. The tasks include creating and managing databases, identifying entities and relationships for a medical center system, designing tables, adding primary keys, enforcing relationships, populating tables with data, and running SQL commands for updating, deleting, and querying relational data. All steps are supported with screenshots as required.

1. A command showing all databases on the system.
![alt text](<Command showing all databases on the system.png>)

1. Create a database and give it your name.

![alt text](<create database.png>)

4. Laikipia University Medical Center Database Design.
   i. Entities:

    - Patients
    - Staff
    - Appointments
    - Treatments
    - Medications

ii. Attributes for each entity:

- Patients: patient_id, name, dob, gender, contact, patient_type (student/staff/visitor)
- Staff: staff_id, name, specialization, contact, hire_date
- Appointments: appointment_id, patient_id, staff_id, date, time, purpose
- Treatments: treatment_id, name, description, cost
- Medications: medication_id, name, dosage, stock_quantity

iii. Relationships:
- Patients have many Appointments (1:M)
- Staff have many Appointments (1:M)
- Appointments may have many Treatments (M:M) - needs junction table
- Treatments may involve many Medications (M:M) - needs junction table

iv. Use a command to display each table’s structure

 - Patients table
 ![alt text](image.png)

- Staffs table 
![alt text](image-1.png)

- Appointments table
  ![alt text](image-2.png)

- Treatments table
  ![alt text](image-3.png)

- Medications table
  ![alt text](image-4.png)

v. For each table, identify the primary key. Use a command to alter the table so as to add a primary key to the table

- Altered Patients table
    ![alt text](<Screenshot from 2025-08-06 15-21-26.png>)

- Altered Staff table
    ![alt text](image-6.png)

- Altered Appointments table
    ![alt text](image-7.png)

- Altered Treatments table
    ![alt text](image-8.png)

- Altered Medications table
    ![alt text](image-9.png)


vi. For each relationship identified in (iii) above, run commands to create the relationship in the database.

  ## Add foreign keys to Appointments and create junction tables for many to many relationships

  ![alt text](image-11.png)

## Show affected tables

  ![alt text](image-12.png)

  ![alt text](image-13.png)

  ![alt text](image-14.png)


  vii. Populate the tables with appropriate entries. Each table should have at least 5 rows.Take a screenshot of each table showing the data entered. [5 marks]

    - Patients table
- ![alt text](image-15.png)

    - Staff table
- ![alt text](image-16.png)
     
    - Appointments table
- ![alt text](image-17.png)
  
    - Treatments table
- ![alt text](image-18.png)
  
    - Medications table
- ![alt text](image-19.png)
 
 Juction tables (Appointment_Treatments and Treatment_Medications)
  
- ![alt text](image-20.png)

viii. Run at least 5 commands to show how you would update data in the table. Take
a screenshot of each command and also the result of the command. [5 marks]

- 1. Update patient contact
  
    ![alt text](image-21.png)

- 2. Change appointment time
  - ![alt text](image-22.png)
  
- 3. Increase medication stock
    ![alt text](image-23.png)

- 4. Change staff specialization
     ![alt text](image-24.png)

- 5. Update treatment cost
  - ![alt text](image-25.png)

ix. Run at least 5 commands to show how to delete data from a table. Take a screenshot of each command and the result of the command. [5 marks]

-- 1. Delete a patient

![alt text](image-30.png)

-- 2. Remove an appointment

  ![alt text](image-29.png)

-- 3. Delete a medication

![alt text](image-28.png)

-- 4. Remove a treatment

![alt text](image-27.png)

-- 5. Delete staff member

-![alt text](image-26.png)

x. For each relationship between two tables in the database, write at least two different commands to show how a join query can be used to fetch data between two related tables simultaneously. Take a screenshot of the query and the output [10 marks]

-- 1. Patients with their appointments

![alt text](image-31.png)

-- 2. Staff with their appointments

![alt text](image-32.png)

-- 3. Appointments with treatments

![alt text](image-33.png)

-- 4. Treatments with medications

![alt text](image-34.png)

-- 5. Patients with their prescribed medications

![alt text](image-35.png)