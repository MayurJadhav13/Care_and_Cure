# Modernizing Healthcare: Care & Cure Hospital Management System

## Problem Statement
The Care & Cure Hospital currently relies on manual record-keeping using books for patient details and tablet management, lacking an online presence. This outdated system results in inefficiencies, data inaccuracies, and limited accessibility for both patients and staff. To address these challenges, the implementation of a comprehensive Hospital Management System (HMS) through a dedicated website is essential.

## Objectives
1. **Digitization of Patient Records:** Transition from manual bookkeeping to a secure, digital platform for storing and managing patient information.
2. **Efficient Tablet Management:** Streamline the process of tablet management, ensuring accurate tracking and timely administration.
3. **Enhanced Accessibility:** Provide a user-friendly website accessible to both hospital staff and patients for seamless interaction with healthcare services.
4. **Cloud Deployment:** Host the system on a cloud platform for scalability, reliability, and easy accessibility.

## Technical Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** PHP
- **Database:** MySQL
- **Cloud Platform:** AWS (Amazon Web Services)

## Local Development Setup
### Prerequisites
- XAMPP
- HTML
- PHP

### Database Setup
1. Create a database named `doctor` in your local MySQL server.
2. Create the following tables:
   - `patient`
   - `tablet`
   - `users` (to store username, password, email)

### Application Pages
- **Login Page:** HTML, CSS
- **Patient Details Page:** HTML, CSS
- **Tablet Info Page:** Included in the patient details page with options to update and check tablet availability.

## Cloud Deployment on AWS
### AWS EC2 Setup
1. **Launch an Instance:**
   - Choose an Ubuntu operating system (22.04 LTS).
   - Instance type: `t2.micro`.
   - Create a key pair.
   - Configure network settings (VPC, IP, security, firewall).

2. **Connect to the Instance:**
   - Use PuTTY to connect to the instance.
   - Username: `ubuntu`.
   - Install necessary packages: MySQL, PHP, Apache.
     ```sh
     sudo apt update
     sudo apt install apache2
     sudo apt install mysql-server
     sudo apt install php libapache2-mod-php php-mysql
     ```
   - Set MySQL username and password.

3. **File Transfer:**
   - Download and install FileZilla.
   - Connect to the server using the public IP address.
   - Transfer your project files to the server.

4. **Configure Apache:**
   - Update MySQL credentials in your PHP code.
   - Ensure necessary PHP extensions (like `mysqli`) are installed.

5. **Access the Application:**
   - Open your browser and navigate to the public IP address of your EC2 instance.
   - If everything is set up correctly, your website should be displayed.

## Additional Notes
- Ensure your PHP code is free of errors for the website to load correctly.
- Regularly back up your database to prevent data loss.

