# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.

---

## 🧪 Choose One Scenario:



### 🔹 Scenario 2: Hospital Database
Design a database for patient management, appointments, medical records, and billing.

**User Requirements:**
- Patient details including contact and insurance.
- Doctors and their departments, contact info, specialization.
- Appointments with reason, time, patient-doctor link.
- Medical records with treatments, diagnosis, test results.
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name
Gokulan R
## Scenario Chosen:
 Hospital 

## ER Diagram:
![Screenshot 2025-05-05 130826](https://github.com/user-attachments/assets/9cfc2d14-0c88-4b56-a45e-4dd1c4d920c7)


## Entities and Attributes:
Patient

Attributes: date of birth, gender, address

Doctor

Attributes: full name, specialization, work schedule

Department

Attributes: department name, department head, department type

Medical Record

Attributes: patient ID, doctor ID, test result

Hospital
(Acts as a central relationship/connection point among other entities.)

## Relationships and Constraints:
Patient — Hospital

Relationship: A patient is associated with a hospital.

Cardinality: Many patients can be associated with one hospital.

Participation: Partial (a patient may or may not be associated with a hospital depending on context).

Doctor — Hospital

Relationship: A doctor works in a hospital.

Cardinality: Many doctors can work in one hospital.

Participation: Total (doctors must be affiliated with a hospital).

Department — Hospital

Relationship: Departments belong to a hospital.

Cardinality: One-to-many (a hospital has many departments).

Participation: Total (each department belongs to a hospital).

Medical Record — Patient, Doctor

Relationship: Each medical record links a patient and a doctor.

Cardinality: Many-to-one for both patient and doctor (each record belongs to one patient and one doctor, but a patient or doctor can have multiple records).

Participation: Total for medical record; partial for patients and doctors.
## Extension (Prerequisite / Billing):
There’s no explicit billing or prerequisite modeling in this diagram. However, to extend it:

Billing could be modeled as a separate entity (e.g., Billing) linked to Patient, Medical Record, or Hospital, with attributes like amount, date, payment method.

Prerequisites for medical procedures or doctor visits could be modeled via a Procedure entity connected to Medical Record or Department.



## Design Choices:
Central Role of Hospital: Hospital is placed centrally to emphasize its role as a hub connecting patients, doctors, departments, and records.

Medical Record as an Associative Entity: It connects patients and doctors and holds specific interaction data (e.g., test results), justifying it as a separate entity rather than an attribute.

Attribute Granularity: Key personal and professional attributes are directly attached to relevant entities for clarity and normalization.

## RESULT
Thus, the Entity-Relationship (ER) Diagram have been created successfully.
