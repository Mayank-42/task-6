Name: Mayank raj
Company:CODTECH IT SOLUTION
ID:CT08DS388
Domain: Java programing
Duration:December 2024to January 2025
Mentor:Muzammil Ahmed      


Overview of the Java Hospital Management System Code
This Java program simulates a hospital management system by managing key aspects such as patient registration, appointment scheduling, electronic health records (EHR), billing, inventory management, and staff management. Below is a detailed breakdown of the code:

1. Patient Class
Attributes:
id, name, age, gender, address, contact, registrationDate
Methods:
Constructor to initialize patient details.
getPatientInfo() method that returns patient details in a formatted string.
2. Appointment Class
Attributes:
appointmentId, patientId, doctorId, appointmentDate, appointmentStatus
Methods:
Constructor to schedule an appointment for a patient with a specific doctor.
getAppointmentDetails() method to return details of an appointment.
cancelAppointment() method to cancel an appointment and update its status.
3. EHR (Electronic Health Records) Class
Attributes:
patientId, medicalHistory (list of medical conditions), prescriptions (list of prescribed medications)
Methods:
addMedicalHistory() and addPrescription() methods to add details to the patient’s medical history or prescriptions.
getEHRDetails() method that formats and returns the patient’s medical history and prescriptions.
4. Billing Class
Attributes:
patientId, services (list of services provided), totalAmount (total bill amount)
Methods:
addService() method to add a service with its cost to the bill.
generateBill() method that formats and returns the final bill for the patient.
5. InventoryItem Class
Attributes:
itemId, name, quantity, price
Methods:
updateQuantity() method to update stock levels of an item.
isLowStock() method to check if the stock is below a threshold (less than 5 items).
getItemDetails() method to return detailed information about an inventory item.
6. Staff Class
Attributes:
staffId, name, role, contact
Methods:
getStaffDetails() method to return detailed information about a staff member.
7. HospitalSystem Class
This is the main class that acts as the core of the system, managing the hospital’s operations.
Attributes:
Maps to store various entities like patients, appointments, ehrRecords, billings, inventory, and staff.
Methods:
Methods for adding and retrieving details of patients, appointments, services, inventory items, and staff members.
checkLowStock() method to check and alert for low stock inventory items.
Methods like registerPatient(), scheduleAppointment(), addServiceToBill(), etc., to handle various operations.
8. Main Class
Purpose: To test and demonstrate the functionality of the HospitalSystem class.
Actions:
Creates a hospital system instance.
Registers patients and staff.
Schedules appointments.
Adds medical services to patient bills.
Adds items to the inventory.
Displays the details of patients, appointments, bills, and inventory.
Checks for low stock in the inventory.
Key Features and Functionality:
Patient Registration: Patients are registered with personal information, and an electronic health record (EHR) is created for each patient.
Appointment Scheduling: Patients can be scheduled for appointments with doctors. Appointments can also be canceled.
EHR Management: Doctors can add medical history and prescriptions for each patient.
Billing: The system generates bills for services provided to patients (e.g., consultations, medical tests).
Inventory Management: Medical supplies are tracked, and low stock levels are flagged.
Staff Management: The system can store information about hospital staff, including doctors and nurses.
How It Works:
Patient Information: Patients are registered with details like name, age, address, and contact.
Appointment Management: Patients can schedule appointments with specific doctors. The appointment can be canceled as needed.
Health Records: As the patient undergoes treatment, their health records are updated with medical history and prescriptions.
Billing: Each service provided to the patient (e.g., consultation, treatment) is added to their bill. The system calculates the total amount due.
Inventory Tracking: Medical supplies such as bandages and syringes are managed. If the stock is low, the system alerts the staff.
Staff Management: Details of hospital staff (doctors, nurses) are stored for easy retrieval.
