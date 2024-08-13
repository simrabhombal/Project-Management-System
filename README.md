# Project Management System Platform

## Overview

Welcome to the Project Management System Platform! This full-stack application is designed to streamline project management tasks, enhance team collaboration, and improve resource allocation. Our platform combines:

### Backend

- **Spring Boot**: 
  Spring Boot simplifies the process of creating production-ready applications with features like:
  - **Auto Configuration**: Minimizes the need for complex XML configuration.
  - **Embedded Servers**: Includes servers like Tomcat, Jetty, or Undertow.
  - **Production Ready**: Built-in support for metrics, health checks, and externalized configuration.
  - **Microservices**: Facilitates microservices architectures with service discovery and circuit breakers.

- **Database**: 
  Utilizes relational databases (e.g., PostgreSQL, MySQL) and Spring Data JPA for:
  - **Data Storage**: Reliable and scalable data management.
  - **Data Access**: Simplifies CRUD operations and complex queries.
    
### Frontend

- **React**: 
  A JavaScript library for building user interfaces with:
  - **Component-Based Architecture**: Modular and reusable components.
  - **Virtual DOM**: Efficiently updates only the changed parts of the UI.
  - **Hooks**: Manages state and side effects in functional components.

- **Shadcn UI**: 
  A UI component library offering:
  - **Customizable Components**: Reusable and customizable UI elements.
  - **Design Consistency**: Ensures a cohesive look and feel.

- **Redux**: 
  A state management library with:
  - **Predictable State**: Centralized state management.
  - **Middleware**: Handles asynchronous actions.
  - **DevTools**: Debugging and state inspection.

- **Tailwind CSS**: 
  A utility-first CSS framework that provides:
  - **Utility-First Approach**: Build custom designs directly in HTML.
  - **Responsive Design**: Easily create responsive layouts.
  - **Customizability**: Configurable design system.
  
## Features

- **User Login**: Secure authentication to access the platform.
- **Homepage**: Centralized dashboard for quick access to projects and tasks.
- **Project Creation**: Create new projects and manage them efficiently.
- **Flash Cards**: Organize project information using flash cards.
- **Member Invitation**: Invite team members to join projects and collaborate.
- **Task Management**: Create, assign, and track tasks within projects.
- **Issue Tracking**: Log and manage issues related to projects.
- **Chat Section**: Real-time communication and collaboration with project members.
- **Subscription Functionality**: Manage and track subscriptions for accessing premium features or services within the platform. Users can subscribe to different tiers based on their needs.


These technologies together provide a comprehensive solution for managing projects and tasks effectively in a modern work environment.

## Getting Started

### Backend

1. **Open the Backend Project:**

   Open the backend project directory in your IDE (e.g., IntelliJ IDEA).

2. **Configure Application Properties:**

   Edit the `src/main/resources/application.properties` file to include your MySQL database credentials and Razorpay API keys. Set the following properties:
   
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
   spring.datasource.username=your_mysql_username
   spring.datasource.password=your_mysql_password
   
   # Razorpay API keys
   razorpay.key.id=your_razorpay_key_id
   razorpay.key.secret=your_razorpay_key_secret
   
3. **Create the Database:**

    Create a new database in MySQL with the name specified in the spring.datasource.url. For example:
    ````bash
      CREATE DATABASE your_database_name;

4. **Build and Run the Backend:**
   Open a terminal in your IDE or navigate to the backend directory and run the following commands:
   ```bash
    ./mvnw clean install
    ./mvnw spring-boot:run

5. Keep the Backend Server Running:
   Ensure that the backend server is running while you work on the frontend.

### Frontend

1. **Navigate to the Frontend Directory:**

   Open a terminal and change to the frontend directory:

   ```bash
   cd path/to/frontend
   //Replace `path/to/frontend` with the actual path to your frontend directory.

2. **Install Dependencies:**
   Install the necessary Node.js dependencies:
   ```bash
   npm install
   
3. Run the Development Server:
   Start the frontend development server:
   ```bash
   npm run dev
   
4. Access the Application:
   Open your browser and navigate to http://localhost:5173 to view the frontend application.
