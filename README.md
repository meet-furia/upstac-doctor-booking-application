# UPSTAC - Doctor Consultation Booking Project

## Overview

This project is a comprehensive application that combines Java Spring for the backend and React for the frontend. It facilitates movie bookings, allowing users to search for movies, view showtimes, book tickets, and manage their bookings.

### Functionality Overview

At its core, this application facilitates movie bookings, allowing users to search for movies, view showtimes, book tickets, and manage their bookings. Here's a detailed breakdown of the application's functionalities:

- **Admin Features:**
  - Admin can add various medical specialists to the application.
  - Admin can retrieve user details.

- **User Features:**
  - Users (patients) can register by filling in their details.
  - Users can log in using their email and password.
  - Users can search for medical specialists and view their available time slots.
  - Users can book appointments with medical specialists.
  - Users can view all the appointments they have made.
  - Users can rate a doctor after their appointment.
  - Users can log out.
## Components

### Frontend

The frontend, built with React, comprises several key components:

1. **Header Component:**
   - **Purpose:** Renders the application header with branding and authentication controls.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState and useEffect.
     - Utilizes Material-UI components for styling and UI elements.
     - Manages user authentication state and handles login/logout functionality.

2. **Appointment Component:**
   - **Purpose:** Displays user appointments and allows them to rate appointments.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState.
     - Fetches user appointments from the backend API and displays them.
     - Integrates modal dialogs for rating appointments seamlessly.

3. **RateAppointment Component:**
   - **Purpose:** Provides a form for users to rate their appointments.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState.
     - Validates user input and submits appointment ratings to the backend API.
     - Utilizes Material-UI components for form elements and styling.

4. **BookAppointment Component:**
   - **Purpose:** Allows users to book appointments with doctors.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState and useEffect.
     - Fetches available time slots from the backend API and handles appointment booking.
     - Integrates date and time pickers for selecting appointment dates and times.

### Backend

1. **Configuration:**
   - **ApiConfiguration:** Instructs Spring-boot to scan the specified package and its sub-packages.
   - **SwaggerConfiguration:** Generates API endpoint documentation.

2. **Constants:** Contains constants used throughout the project.

3. **Controllers:** Contains endpoints and their corresponding responses.

4. **Entities:** Contains entity classes used throughout the project.

5. **Enums:**
   - **Specialty:** Enumerates various specialties.
   - **UserAuthTokenStatus:** Enumerates authentication token status values.

6. **Exceptions:** Contains classes that handle various types of exceptions.

7. **Handler:**
   - **RestExceptionHandler:** Handles specific exceptions and sends responses to users.

8. **Models:**
   - **AuthorizedUser:** POJO containing authorized user information.
   - **TimeSlot:** Provides available time slots.

9. **Providers:**
   - **BasicAuthDecoder:** Decodes email and password.
   - **BearerAuthDecoder:** Decodes authentication tokens.
   - **PasswordCryptographyProvider:** Hashes and salts passwords for security.
   - **TokenCrytographyProvider:** Encrypts and decrypts tokens.

10. **Token Providers:**
    - **JwtTokenProvider:** Generates authentication tokens.
    - **Token:** Specification defining generated tokens.
    - **TokenProvider:** Declares methods for serializing and deserializing tokens.

11. **Repository:** Provides CRUD operations for interacting with the database.

12. **Services:**
    - **AppointmentService:** Saves and retrieves appointments.
    - **AuthenticationService:** Authenticates users and generates tokens.
    - **AuthTokenService:** Manages token generation, validation, and invalidation.
    - **DoctorService:** Registers doctors, retrieves doctor information, and manages ratings and time slots.
    - **RatingsService:** Manages ratings and calculates average ratings.
    - **UserAuthTokenVerifier:** Stores token status.
    - **UserService:** Registers users, retrieves user information, and manages user-related operations.

13. **Utilities:**
    - **ValidationUtils:** Provides code for validating user, doctor, and appointment details.


markdown
Copy code
# Movie Booking Application Project

## Overview

In this segment, you will dive deeper into the project.

### Functionality Overview

At its core, this application facilitates movie bookings, allowing users to search for movies, view showtimes, book tickets, and manage their bookings. Here's a detailed breakdown of the application's functionalities:

- **Admin Features:**
  - Admin can add various medical specialists to the application.
  - Admin can retrieve user details.

- **User Features:**
  - Users (patients) can register by filling in their details.
  - Users can log in using their email and password.
  - Users can search for medical specialists and view their available time slots.
  - Users can book appointments with medical specialists.
  - Users can view all the appointments they have made.
  - Users can rate a doctor after their appointment.
  - Users can log out.

## Components

### Backend

1. **Configuration:**
   - **ApiConfiguration:** Instructs Spring-boot to scan the specified package and its sub-packages.
   - **SwaggerConfiguration:** Generates API endpoint documentation.

2. **Constants:** Contains constants used throughout the project.

3. **Controllers:** Contains endpoints and their corresponding responses.

4. **Entities:** Contains entity classes used throughout the project.

5. **Enums:**
   - **Specialty:** Enumerates various specialties.
   - **UserAuthTokenStatus:** Enumerates authentication token status values.

6. **Exceptions:** Contains classes that handle various types of exceptions.

7. **Handler:**
   - **RestExceptionHandler:** Handles specific exceptions and sends responses to users.

8. **Models:**
   - **AuthorizedUser:** POJO containing authorized user information.
   - **TimeSlot:** Provides available time slots.

9. **Providers:**
   - **BasicAuthDecoder:** Decodes email and password.
   - **BearerAuthDecoder:** Decodes authentication tokens.
   - **PasswordCryptographyProvider:** Hashes and salts passwords for security.
   - **TokenCrytographyProvider:** Encrypts and decrypts tokens.

10. **Token Providers:**
    - **JwtTokenProvider:** Generates authentication tokens.
    - **Token:** Specification defining generated tokens.
    - **TokenProvider:** Declares methods for serializing and deserializing tokens.

11. **Repository:** Provides CRUD operations for interacting with the database.

12. **Services:**
    - **AppointmentService:** Saves and retrieves appointments.
    - **AuthenticationService:** Authenticates users and generates tokens.
    - **AuthTokenService:** Manages token generation, validation, and invalidation.
    - **DoctorService:** Registers doctors, retrieves doctor information, and manages ratings and time slots.
    - **RatingsService:** Manages ratings and calculates average ratings.
    - **UserAuthTokenVerifier:** Stores token status.
    - **UserService:** Registers users, retrieves user information, and manages user-related operations.

13. **Utilities:**
    - **ValidationUtils:** Provides code for validating user, doctor, and appointment details.

### Frontend

1. **Header Component:**
   - **Purpose:** Renders the application header with branding and authentication controls.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState and useEffect.
     - Utilizes Material-UI components for styling and UI elements.
     - Manages user authentication state and handles login/logout functionality.

2. **Appointment Component:**
   - **Purpose:** Displays user appointments and allows them to rate appointments.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState.
     - Fetches user appointments from the backend API and displays them.
     - Integrates modal dialogs for rating appointments seamlessly.

3. **RateAppointment Component:**
   - **Purpose:** Provides a form for users to rate their appointments.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState.
     - Validates user input and submits appointment ratings to the backend API.
     - Utilizes Material-UI components for form elements and styling.

4. **BookAppointment Component:**
   - **Purpose:** Allows users to book appointments with doctors.
   - **Technical Details:**
     - Implemented using React functional components and hooks like useState and useEffect.
     - Fetches available time slots from the backend API and handles appointment booking.
     - Integrates date and time pickers for selecting appointment dates and times.

### MySQL Database


The MySQL database serves as the persistent storage layer for the application:

1. **Address Table:**
   - Stores address details for users.

2. **Appointment Table:**
   - Records appointments made by users with doctors.

3. **Doctor Table:**
   - Stores information about medical specialists.

4. **UserAuthToken Table:**
   - Stores authentication tokens generated for users upon login.

5. **User Table:**
   - Records user details for authentication and identification purposes.

6. **Ratings Table:**
   - Stores ratings provided by users for doctors.


## Conclusion

This application provides a comprehensive platform for medical consultation, facilitating interactions between patients and medical specialists. By leveraging technologies such as Java Spring for the backend, React for the frontend, and MySQL for data storage, it offers a seamless and intuitive user experience. Users can register, log in, search for doctors, book appointments, rate doctors, and manage their appointments efficiently. With its robust functionality and user-friendly interface, the application aims to streamline the process of accessing medical care and improving patient-doctor interactions.
