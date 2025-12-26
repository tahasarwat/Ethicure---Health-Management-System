# ETHICURE - Your Heathhub Manager
Group Project-
Hospital Management System
Hospital Management System using MySQL, Php and Bootstrap


## Features to Implement:

1) Appointment Approval: Enable doctors to accept appointments and notify patients of approval.
2) Email Validation: Prevent users from registering with an already registered email ID.
3) Password Security: Ensure passwords are encrypted and not displayed in the admin panel.
4) Pagination: Implement pagination for all list views across the application.
5) Bug Fix - Bill Payment Receipt: Ensure the receipt does not contain multiple records for a patient associated with the same doctor multiple times.
6) Prescription Details: Add more fields to prescription statements for specificity.
7) Payment Details: Include additional details such as the date of payment and the amount paid.
8) Export Functionality: Add an export button in the admin module to export all details to an Excel sheet.

## Prerequisites
1. Install XAMPP web server
2. Any Editor 
3. Any web browser with latest version

## Languages and Technologies used
1. HTML5/CSS3
2. JavaScript (to create dynamically updating content)
3. Bootstrap (An HTML, CSS, and JS library)
4. XAMPP (A web server by Apache Friends)
5. PhP
6. MySQL (An RDBMS that uses SQL)
7. TCPDF (to generate PDFs)

## Steps to run the project in your machine
1. Download and install XAMPP in your machine
2. Clone or download the repository
3. Extract all the files and move it to the 'htdocs' folder of your XAMPP directory.
4. Start the Apache and Mysql in your XAMPP control panel.
5. Open your web browser and type 'localhost/phpmyadmin'
6. In phpmyadmin page, create a new database from the left panel and name it as 'myhmsdb'
7. Import the file 'myhmsdb.sql' inside your newly created database and click ok.
8. Open a new tab and type 'localhost/foldername' in the url of your browser

    
### SOFTWARES USED
  - XAMPP was installed on the Ubuntu 19.04 machine and APACHE2 Server and MySQL were initialized. And, files were built inside opt/lampp/htdocs/myhmsp
  - Sublime Text 3.2 was used as a text editor.
  - Google Chrome Version 77.0.3865.90 was used to run the project (localhost/myhmsp was used as the url).
  

### Starting Apache And MySQL in XAMPP:
  The XAMPP Control Panel allows you to manually start and stop Apache and MySQL. To start Apache or MySQL manually, click the ‘Start’ button under ‘Actions’.
  
  
![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/cf5fc5ee-580a-4b2e-bb87-9f7272913778)



## GETTING INTO THE PROJECT:
The system includes a ‘Home’ page where patients, doctors, and administrators can log in to their accounts. Below is a visual guide to the system's main features and modules.


![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/785cac00-3f2c-4f91-aa28-71feabf0beff)



'About Us' page allows us to get some more information about the quality and the services of the hospital.

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/7d87781d-fad0-4dbc-8913-83196dbe0005)


![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/c84158d0-ba47-4d90-be09-ed26ca16879a)



‘Contact’ page allows users to provide feedback or queries about the services of the hospital. Fig below shows the ‘Contact’ page.

  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/40386351-4cb1-4d8a-b1fd-b4b69bc2da26)



The ‘Home’ page consists of 3 modules:
1. Patient Module
2. Doctor Module
3. Admin Module

### Patient Module:

  &nbsp; &nbsp; &nbsp; This module allows patients to create their account, book an appointment to see a doctor and see their appointment history.
  The registration page(in the home page itself) asks patients to enter their First Name, Last Name, Email ID, Contact Number, Password and radio buttons to select their gender.
  
  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/2f7deea0-ecd0-40fe-ad8e-4bd18a26d104)



Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard.

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/93e2f76c-3d1f-4f01-8517-f8fb49964e37)



The Dashboard page allows patients to perform two operations:

**1. Book his/her appointment:**

  &nbsp; &nbsp; &nbsp; Here, the patients can able to book their appointments to see a doctor. The appointment form requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/9896631c-15b5-4942-83ec-d92055044732)



After clicking on the ‘Create new entry’ button, the patient will receive an alert that acknowledges the successful appointment of the patient.


**2. View patients’ Appointment History:**

  &nbsp; &nbsp; &nbsp; Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.
	
![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/2ff79bd0-e19d-4a0d-b300-18047ababc81)



Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again. Fig below shows the login page.
Clicking on ‘Login’ button will redirect the patient to his dashboard page which we have seen earlier.

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/613eadab-dffa-414c-8d99-c026df474bb7)



This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history.

### Doctor Module:

  &nbsp; &nbsp; &nbsp; The doctors can login into their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’. Registration of a doctor account can be done only by admin. We will discuss more about this in Admin Module.
  
![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/693161f2-3ac9-4e90-bd06-feb7b28cadd2)



Once the doctor clicking the ‘Login’ button, they will be redirected to their own dashboard.

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/f626e6b7-7ebd-42e7-bed6-537a54d00a3f)



In this page, doctor can able to see their appointments which has been booked by the patients.

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/b753753c-962e-4cda-8496-5a0420dadd4b)



In real-time, the doctors will have thousands of appointments. It will be easier for a doctor to search for appointment in the case of more appointments. To make it easier, I have a ‘Search’ box in the navigation bar which allows doctors to search for a patient by their contact number.
&nbsp; &nbsp; &nbsp; Once everything is done, the doctor can logout of their account. Thus, in general, a doctor can login into his/her account, view their appointments and search for a patient. This is all about Doctor Module.

### Admin Module:
   
   &nbsp; &nbsp; &nbsp; This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments and the feedback/queries received from the ‘Contact’ page. Also admin can add doctor too. 
  &nbsp; &nbsp; &nbsp; Login into admin account can be done by toggling into admin tab of the Home page. 
  &nbsp; &nbsp; &nbsp; `username`: admin, `password`: admin123

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/d2464951-25fd-488a-b24f-c28305bfa00c)



On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard 

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/ccea192d-7192-4fbe-979b-06ac87750cba)



This module allows admin to perform five major operations:

**1. View the list of all patients registered:**

  &nbsp; &nbsp; &nbsp; Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password.As like in doctor module, admin can also search for a patient by their contact number in the search box.
  
  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/44d4f1b5-1f98-4912-af19-c09c95f36dbb)


  
**2. View the list of all doctors registered:**

  &nbsp; &nbsp; &nbsp; Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees. Searching for a doctor can be done by using the doctor’s Email ID in the search box.

![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/fe4755aa-37d4-4c39-904c-d0bee03cfa54)



**3. View the Appointment lists:**

  &nbsp; &nbsp; &nbsp; Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. 

  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/cb80ccd6-32f8-4a2c-823c-8c87f53c5905)


  
 **4. Add Doctor:**

  &nbsp; &nbsp; &nbsp; Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.
  
  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/a8a9bbc9-6dd1-4289-a56c-a905d22ae231)


  
  After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the list.
  
 ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/7df5be54-f26f-4502-90b7-255ec7aeca40)


  
**5. View User’s feedback/Queries:**

  &nbsp; &nbsp; &nbsp; Admin is allowed to view the feedback/Query that has been given by the user in the ‘Contact’ page. This includes User’s Name, Email Id, Contact Number and the message(Feedback/ Query).

  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/531b2aa1-2c78-4db0-83f0-0fa899dff745)


 **6. Delete Doctor:**

  &nbsp; &nbsp; &nbsp; Admin is allowed to Delete a previously added doctor.

  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/d066c94b-310f-4685-ab13-2d70d48fee08)


  After deleting a doctor we can see that he/she is removed from the doctor list.

  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/626acd72-7c4e-44f1-8aa8-1b0688579107)


  **7. View Prescription List for User:**

  &nbsp; &nbsp; &nbsp; Admin is allowed to view the Prescription List that has been given to the user by the doctor. 

  ![image](https://github.com/Kshitijboi/EthiCure/assets/116621388/abc3660d-4c36-4047-9471-1e44379edeee)




  &nbsp; &nbsp; &nbsp; Taking everything into consideration, admin can able to view the details of patients and doctors, appointment details, Feedback by the user, add a new doctor, delete an existing doctor and 
  checking the Prescription List. Once everything is done, the admin can logout from his account.

  ** This was Ethicure Your Personal HealthHub Manager which manages everything related to your medication.**







