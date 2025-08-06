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
