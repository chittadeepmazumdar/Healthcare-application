
# HealthCare-Application

## 🩺 Overview
A Java-based backend system for managing healthcare workflows including users, doctors, appointments, payments, and notifications. Designed using Spring Boot and layered architecture to ensure modularity, scalability, and security.

---

## 📦 Package Structure

### ✅ Root Packages
- `BackendApplication.java`: Entry point for launching the Spring Boot application.

### 📂 `com.healthcare.controller`
Handles incoming HTTP requests and maps them to service calls:
- `AdminController.java`
- `AppointmentController.java`
- `DoctorController.java`
- `NotificationController.java`
- `PaymentController.java`
- `UserController.java`

### 📂 `com.healthcare.dto`
Encapsulates data transfer between layers and client:
- `ApiResponse.java`
- `AppointmentDto.java`
- `ForgotPasswordDTO.java`
- `PaymentRequestDTO.java`
- `PaymentResponseDTO.java`
- `SigninResponse.java`

### 📂 `com.healthcare.entities`
JPA entities and enums used for ORM mapping:
- Domain Entities: `Appointment.java`, `Doctor.java`, `Payment.java`, `Role.java`, `User.java`
- Enums: `AppointmentStatus`, `NotificationStatus`, `PaymentStatus`, `PaymentMethod`

### 📂 `com.healthcare.exceptions`
Handles custom error definitions:
- `EntityNotFoundException.java`
- `ResourceNotFoundException.java`

### 📂 `com.healthcare.repository`
Spring Data JPA interfaces for DB access:
- `AppointmentRepository.java`
- `DoctorRepository.java`
- `NotificationRepository.java`
- `PaymentRepository.java`
- `UserRepository.java`

### 🔒 `com.healthcare.security`
Implements JWT-based authentication and authorization:
- `SecurityConfig.java`
- `JwtUtils.java`
- `CustomJwtAuthenticationFilter.java`
- `CustomAuthenticationEntryPoint.java`
- `CustomUserDetails.java`
- `CustomUserDetailsService.java`

### ⚙️ `com.healthcare.service`
Business logic layer organized into interfaces and implementations:
- Appointments: `AppointmentService.java`, `AppointmentServiceImpl.java`
- Doctors: `DoctorService.java`, `DoctorServiceImpl.java`
- Notifications: `NotificationService.java`, `NotificationServiceImpl.java`
- Payments: `PaymentService.java`, `PaymentServiceImpl.java`
- Users: `UserService.java`, `UserServiceImpl.java`
- Utilities: `EmailService.java`, `SmsService.java`

---

## 🧪 Technologies Used

- Java 17+
- Spring Boot
- Spring Security (JWT)
- Hibernate
- Maven

---

## 📌 Features

- Secure authentication via JWT
- Role-based access control
- CRUD operations for Users, Doctors, Appointments
- Integrated email and SMS notifications
- Payment handling & response tracking

---

## 🚀 Getting Started

### Prerequisites
- Java 17 or higher
- Maven

### Setup

```bash
# Clone the repository
git clone https://github.com/your-username/HealthCare-Application.git

# Change directory
cd HealthCare-Application

# Build the project
mvn clean install

# Run the application
mvn spring-boot:run
```

### Configuration
- Database and environment variables can be set in `application.properties` or `application.yml`.
- JWT secret and other sensitive configs should be managed securely.

---

## 👨‍💻 Contributing

Contributions are welcome! Please open an issue or submit a pull request for suggested improvements.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 📬 Contact

For questions or feedback, reach out via [GitHub Issues](https://github.com/your-username/HealthCare-Application/issues).

On Thu, Jul 31, 2025 at 1:52 PM Twinkle kumar <twinklekumar.iacsd@gmail.com> wrote:


---------- Forwarded message ---------
From: Twinkle kumar <twinklekumar.iacsd@gmail.com>
Date: Thu, Jul 31, 2025 at 1:50 PM
Subject: description of the project (readme)
To: <iacdsvedang@gmail.com>


# HealthCare-Application

## 🩺 Overview
A Java-based backend system for managing healthcare workflows including users, doctors, appointments, payments, and notifications. Designed using Spring Boot and layered architecture to ensure modularity, scalability, and security.

## 📦 Package Structure

### ✅ Root Packages
- `BackendApplication.java`: Entry point for launching the Spring Boot application.

### 📂 `com.healthcare.controller`
Handles incoming HTTP requests and maps them to service calls:
- `AdminController.java`
- `AppointmentController.java`
- `DoctorController.java`
- `NotificationController.java`
- `PaymentController.java`
- `UserController.java`

### 📂 `com.healthcare.dto`
Encapsulates data transfer between layers and client:
- `ApiResponse.java`, `AppointmentDto.java`, `ForgotPasswordDTO.java`, `PaymentRequestDTO.java`, `PaymentResponseDTO.java`, `SigninResponse.java`

### 📂 `com.healthcare.entities`
JPA entities and enums used for ORM mapping:
- Domain Entities: `Appointment.java`, `Doctor.java`, `Payment.java`, `Role.java`, `User.java`
- Enums: `AppointmentStatus`, `NotificationStatus`, `PaymentStatus`, `PaymentMethod`

### 📂 `com.healthcare.exceptions`
Handles custom error definitions:
- `EntityNotFoundException.java`
- `ResourceNotFoundException.java`

### 📂 `com.healthcare.repository`
Spring Data JPA interfaces for DB access:
- `AppointmentRepository.java`
- `DoctorRepository.java`
- `NotificationRepository.java`
- `PaymentRepository.java`
- `UserRepository.java`

### 🔒 `com.healthcare.security`
Implements JWT-based authentication and authorization:
- `SecurityConfig.java`
- `JwtUtils.java`
- `CustomJwtAuthenticationFilter.java`
- `CustomAuthenticationEntryPoint.java`
- `CustomUserDetails.java`
- `CustomUserDetailsService.java`

### ⚙️ `com.healthcare.service`
Business logic layer organized into interfaces and implementations:
- Appointments: `AppointmentService.java`, `AppointmentServiceImpl.java`
- Doctors: `DoctorService.java`, `DoctorServiceImpl.java`
- Notifications: `NotificationService.java`, `NotificationServiceImpl.java`
- Payments: `PaymentService.java`, `PaymentServiceImpl.java`
- Users: `UserService.java`, `UserServiceImpl.java`
- Utilities: `EmailService.java`, `SmsService.java`
🧪 Technologies Used
Java 17+
Spring Boot
Spring Security (JWT)
Hibernate
Maven
📌 Features

Secure authentication via JWT
Role-based access control
CRUD operations for Users, Doctors, Appointments
Integrated email and SMS notifications
Payment handling & response tracking