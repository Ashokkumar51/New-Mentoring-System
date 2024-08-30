New Mentoring System

## Overview

The Mentoring System is a web-based application designed to facilitate mentorship programs within an organization. It enables mentors and mentees to connect, schedule meetings, and track progress. The application is built using Java Servlets and JSP (JavaServer Pages) for dynamic web content, and follows the MVC (Model-View-Controller) architecture for clean separation of concerns.

## Features

- **User Authentication**: Secure login and registration for mentors and mentees.
- **Profile Management**: Users can create and update their profiles with relevant information.
- **Mentor-Mentee Matching**: Algorithmic matching based on interests and expertise.
- **Scheduling**: Ability to schedule and manage meetings.
- **Progress Tracking**: Tracking mentorship progress through feedback and notes.

## Technology Stack

- **Backend**: Java Servlets
- **Frontend**: JSP, HTML, CSS, JavaScript
- **Database**: MySQL
- **Server**: Apache Tomcat
- **Build Tool**: Apache Maven

## Prerequisites

- Java Development Kit (JDK) 11 or higher
- Apache Maven 3.6+
- Apache Tomcat 9.0+
- MySQL 8.0+
- A modern web browser (Chrome, Firefox, etc.)

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Ashokkumar51/mentoring-system.git
   cd mentoring-system
   ```

2. **Configure the database:**
   - Create a MySQL database named `mentoring_system`.
   - Import the provided SQL script to create the necessary tables.
     ```sh
     mysql -u root -p mentoring_system < database/schema.sql
     ```

3. **Update database credentials:**
   - Edit the `src/main/resources/db.properties` file with your MySQL username and password.
     ```properties
     db.url=jdbc:mysql://localhost:3306/mentoring_system
     db.username=root
     db.password=yourpassword
     ```

4. **Build the project:**
   ```sh
   mvn clean install
   ```

5. **Deploy to Tomcat:**
   - Copy the generated WAR file from the `target` directory to the `webapps` directory of your Tomcat installation.
   - Start Tomcat server.

6. **Access the application:**
   - Open a web browser and go to `http://localhost:8080/mentoring-system`.

## Usage

### User Registration

- Navigate to the registration page.
- Fill in the required information and submit.
- Upon successful registration, you will be redirected to the login page.

### User Login

- Enter your credentials on the login page.
- Upon successful login, you will be redirected to your dashboard.

### Profile Management

- Access your profile through the dashboard.
- Update your personal information and preferences as needed.

### Mentor-Mentee Matching

- Complete your profile to help the system match you with suitable mentors or mentees.
- View suggested matches and send/receive requests.

### Tracking Progress

- Add notes and feedback after each meeting.
- Track your progress and milestones throughout the mentorship program.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code follows the project's coding standards and includes appropriate tests.

## Contact

For any questions or suggestions, please contact (mailto:soutapalliab@gmail.com).

---

This README file provides a clear and concise guide to setting up and using the Mentoring System application. It includes all necessary information for installation, configuration, and usage, making it easy for new users to get started.
