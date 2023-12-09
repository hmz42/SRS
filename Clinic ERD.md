# Clinic Reservation System Documentation

## Overview

This repository contains the database schema and relationships for a clinic reservation system. The system involves entities such as Patient, Doctor, Appointment, Payment, MedicalRecord, InsuranceProvider, and Specialty. Below is a detailed explanation of each entity, its attributes, and the relationships between them.

## Entities

1. **Patient:**
   - PatientID (PK)
   - FirstName
   - LastName
   - DateOfBirth
   - Gender
   - Email
   - Phone
   - Address
   - InsuranceInformation
   - EmergencyContactName
   - EmergencyContactPhone

2. **Doctor:**
   - DoctorID (PK)
   - FirstName
   - LastName
   - Specialization
   - Email
   - Phone
   - OfficeLocation
   - WorkingDays
   - WorkingHours

3. **Appointment:**
   - AppointmentID (PK)
   - PatientID (FK)
   - DoctorID (FK)
   - AppointmentDate
   - StartTime
   - EndTime
   - Status

4. **Payment:**
   - PaymentID (PK)
   - AppointmentID (FK)
   - Amount
   - PaymentDate
   - PaymentMethod
   - TransactionID

5. **MedicalRecord:**
   - RecordID (PK)
   - PatientID (FK)
   - DoctorID (FK)
   - AppointmentID (FK)
   - Diagnosis
   - Prescription
   - Notes
   - Date
   - FollowUpDate

6. **InsuranceProvider:**
   - InsuranceProviderID (PK)
   - ProviderName
   - CoverageDetails
   - ContactNumber
   - Email

7. **Specialty:**
   - SpecialtyID (PK)
   - SpecialtyName
   - Description

## Relationships

1. **Patient-Appointment (1 to M):**
   - Patient.PatientID → Appointment.PatientID

2. **Doctor-Appointment (1 to M):**
   - Doctor.DoctorID → Appointment.DoctorID

3. **Appointment-Payment (1 to 1):**
   - Appointment.AppointmentID → Payment.AppointmentID

4. **Patient-MedicalRecord (1 to M):**
   - Patient.PatientID → MedicalRecord.PatientID

5. **Doctor-MedicalRecord (1 to M):**
   - Doctor.DoctorID → MedicalRecord.DoctorID

6. **Appointment-MedicalRecord (1 to 1):**
   - Appointment.AppointmentID → MedicalRecord.AppointmentID

7. **Patient-InsuranceProvider (M to 1):**
   - Patient.InsuranceProviderID → InsuranceProvider.InsuranceProviderID

8. **Doctor-Specialty (M to 1):**
   - Doctor.SpecialtyID → Specialty.SpecialtyID

Note: Adjustments can be made based on specific requirements and features of your clinic reservation system. Please refer to this documentation to understand the relationships and key attributes for each entity. If there are any changes or additional features needed, update the schema accordingly.
