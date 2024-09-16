## CU Visitor Management System

### Login System:
- Separate login options for three user types: Security, Teacher, and Chief Security.
- Role-based access ensures that each user can only access the features assigned to their role.

### Visitor Form Submission:
- Teachers can submit a form detailing the visitor's information such as name, purpose of visit, and date.
- The data is stored in Firebase Realtime Database, allowing easy access for validation and security purposes.

### Chief Security Role:
- The Chief Security (Admin) can review the forms submitted by teachers and either approve or reject them.
- Approved visitors receive a parking slot assignment, and a QR code is generated.
- The QR code is automatically emailed to the visitor upon approval.

### Security Role:
- Security personnel have access to the visitor's details to validate entries.
- QR codes are scanned upon the visitor's arrival, verifying the data and allowing seamless check-in.
- For walk-in visitors, Security can manually add their information into the system.

### Visitor QR Code:
- A QR code is generated once the Chief Security approves the visitor’s form. This QR code is used by the security team for quick verification during check-in.

### Database Integration:
- All visitor data, approval status are stored and managed in Firebase Realtime Database.
- Firebase also handles storage for any relevant files, such as profile photos or documents.

### User Interface:
- The app uses clean and intuitive UI elements like menus, navigation drawers, and intents to provide smooth navigation between different sections.
- Form validation ensures proper submission of details, including email, phone number, and date formats.

### Walk-In Visitor Management:
- Security personnel can add and manage walk-in visitors on-site, ensuring real-time data entry and smooth handling of unexpected visits.
