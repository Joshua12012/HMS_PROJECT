# AI-Powered WhatsApp Chatbot for Hospital Management System  

## Overview  
This project introduces an AI-based WhatsApp chatbot designed to simplify appointment booking and provide patients and their families with essential healthcare information. The chatbot supports multilingual conversations in **English**, **Marathi**, and **Hindi**, ensuring accessibility for a broad audience.  

The system combines state-of-the-art technologies for natural language processing, secure communication, and efficient database management, making it a robust solution for healthcare institutions.  

---

## Features  
- **Multilingual Support**: Communicates in English, Marathi, and Hindi.  
- **Appointment Management**: Enables booking, modification, and cancellation of appointments.  
- **Information Access**: Provides detailed hospital-related information.  
- **Secure Data Management**: Protects patient data with reliable storage solutions.  

---

## Technology Stack  
- **Groq API**: Natural language processing (NLP) for understanding and responding to user queries.  
- **Twilio**: Facilitates seamless WhatsApp connectivity.  
- **Ngrok**: Provides secure HTTPS tunneling for reliable connections.  
- **MySQL**: Stores and manages patient appointment data efficiently.  

---

## Installation and Setup  

### Prerequisites  
Before setting up the application, ensure you have the following:  
1. **Python**: Installed on your system.  
2. **MySQL**: A running MySQL server instance.  
3. **Accounts for Services**: Sign up for:  
   - [Twilio](https://www.twilio.com/)  
   - [Ngrok](https://ngrok.com/)  
   - [Groq API](https://groq.com/).  
4. **Dependencies**: Install required Python libraries.  

---

### Steps to Set Up  

1. **Clone the Repository**  
   Download the project repository to your local machine:  
   ```bash
   git clone https://github.com/HMS_PROJECT/hospital-management-chatbot.git
   cd HMS_PROJECT
2. Install Dependencies
   Install the necessary Python libraries using the following command:
   ```bash
   pip install -r requirements.txt
3. Set Up the MySQL Database
  Open MySQL Workbench or a terminal and create a database named hospital_management.
  Import the provided database schema:
  ```bash
    mysql -u username -p hospital_management < database/schema.sql
  ```
  Update the config.py file with your MySQL credentials (username, password, and database name).
  
4. Configure Twilio for WhatsApp

   Sign in to your Twilio account and create a new WhatsApp-enabled number.
   Copy your Twilio Account SID, Auth Token, and WhatsApp number.
   Add these details to the config.py file.
5. Set Up Ngrok
   Download and install Ngrok.
   Start an Ngrok tunnel to expose your local Flask application:
   ```bash
    ngrok http 5000
   ```
   Copy the HTTPS URL provided by Ngrok and add it as a webhook in your Twilio account.
6. Run the Flask Application
   Start the chatbot application by running:
   ``` bash
   python app.py
   ```
   
7. Test the Chatbot
   Send a message to your Twilio WhatsApp number.
   The chatbot will guide you through booking, modifying, or canceling an appointment.

## Summary
The AI-powered WhatsApp chatbot offers a user-friendly, efficient, and secure solution for managing hospital appointments and providing healthcare-related information. By leveraging advanced technologies such as Groq API, Twilio, Ngrok, and MySQL, the system ensures seamless communication and robust data management.

This project represents a significant step forward in healthcare automation, enhancing accessibility and operational efficiency for both patients and healthcare providers.
