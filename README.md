# Hospital Management System

A comprehensive Hospital Management System (HMS) project designed to streamline and enhance the administrative and operational functions of hospitals using PHP, MySQL, HTML, CSS, JavaScript, and Bootstrap. Developed for the Department of Information Technology, CMR Engineering College.

***

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Database Design](#database-design)
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Conclusion](#conclusion)
- [References](#references)

***

## Introduction

The Hospital Management System (HMS) aims to improve the efficiency of healthcare delivery by integrating crucial processes like patient data management, doctor scheduling, appointment booking, billing, inventory, and reporting[1]. This system enables centralized, secure, and easy access to patient and hospital information, reduces manual workload, and helps in delivering timely, personalized care.

***

## Features

- Patient registration and record management
- Doctor, nurse, and administrator information management
- Appointment scheduling and management
- Automated billing and payment tracking
- Medical record storage (diagnosis, treatment, medications)
- Inventory tracking of medical supplies
- User-friendly web interface using HTML & Bootstrap
- Automated generation of essential hospital reports[1]

***

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript, Bootstrap
- **Backend:** PHP
- **Database:** MySQL Server (XAMPP-based)
- **Supported OS:** Windows 7/8/9/10[1]

***

## Database Design

### Main Entities

| Entity | Attributes |
| -------------- | ---------- |
| Patient | patientID (PK), name, gender, dateOfBirth, contactDetails |
| Doctor | doctorID (PK), name, specialization, contactDetails |
| Nurse | nurseID (PK), name, department, contactDetails |
| Administrator | adminID (PK), name, department, contactDetails |
| Department | deptID (PK), name, headDoctor, numOfBeds |
| Appointment | appointmentID (PK), patientID (FK), doctorID (FK), appointmentDate, appointmentTime, status |
| MedicalRecord | recordID (PK), patientID (FK), doctorID (FK), diagnosis, medications, treatment |

### Key Relationships

- One-to-Many: Patient–Appointment, Doctor–Appointment, Patient–MedicalRecord, Doctor–MedicalRecord, Doctor–Department, Nurse–Department, Admin–Department[1].

***

## Installation

1. **Clone the Repository:**
   ```
   git clone https://github.com/yourusername/hospital-management-system.git
   ```
2. **Install XAMPP:**  
   Download and install [XAMPP](https://www.apachefriends.org/index.html) and ensure Apache and MySQL modules are running.

3. **Setup Database:**
   - Import the database schema found in the `/database` folder to your local MySQL server:
   - Use the provided SQL script to create the `hospitalmanagement` database and required tables[1].

4. **Configure Project Files:**
   - Place the project folder inside XAMPP's `/htdocs` directory.
   - Edit database connection settings in PHP files as needed (hostname: `localhost`, user: `root`, password: ``, database: `hospitalmanagement`).

5. **Run the Application:**
   - Open your browser and go to `http://localhost/hospital-management-system/`[1].

***

## Usage

- Use the navigation bar to perform actions:
  - Add, view, and search for patients
  - Manage doctor and staff records
  - Schedule appointments
  - Enter and view medical records
  - Initiate and record billing procedures
  - Manage inventory and view reports[1]

***

## Screenshots

- **Home Page:** Main interface of the system
- **Add Patient Page:** Entering new patient details
- **View Patients:** Display of all registered patients

(Include actual screenshots here in your GitHub repo.)

***

## Conclusion

Implementing this HMS boosts efficiency, security, and reliability of hospital operations by automating data management and administrative tasks. It empowers healthcare providers with the tools to deliver better patient outcomes and enhanced hospital performance[1].

***

## References

- R. Batra and A. S. Pall, "Barriers to adoption of hospital management systems: A study of Punjab healthcare industry," Prabandhan Indian Journal of Management, vol. 9, no. 11, 2016.
- R. G. Misal, "Advanced Hospital Management System," Int J Res Appl Sci Eng Technol, vol. 10, no. 6, 2022.
- P. K. Yadav and R. Kumar, "Online Hospital Management System," SSRN Electronic Journal, 2022[1].

***

Feel free to update this README with additional details like contributors, demo video links, or more usage notes as necessary.

Citations:
[1] DBMS-INDIVIDUAL-PROJECT-3.pdf https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/84486606/cefa95d8-5da6-4fe6-a8ac-e983a7c36522/DBMS-INDIVIDUAL-PROJECT-3.pdf

