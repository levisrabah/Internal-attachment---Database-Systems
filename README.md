1. Internal attachment : Database Systems

2. A command showing all databases on the system.
![alt text](<Command showing all databases on the system.png>)

3. Create a database and give it your name.

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
