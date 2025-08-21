# Airbnb Clone Project

## Brief Overview of the Project
This project is an **Airbnb clone** that provides core functionalities such as **user authentication, property listings, bookings, payments, and reviews**.  
The goal is to simulate a real-world property rental system while practicing **backend system design, API development, and DevOps deployment pipelines**.

---

### Goals
- Build a **scalable property rental platform** similar to Airbnb.  
- Implement **RESTful APIs** for authentication, property management, booking, payment, and reviews.  
- Ensure **database optimization** for performance and scalability.  
- Deploy the application with **CI/CD pipelines** for continuous integration and delivery.  
- Provide **secure APIs** with authentication and authorization.

---

### Technology Stack
- **Backend Framework:** Node.js (Express / TSOA) or Python (Flask/Django)  
- **Database:** PostgreSQL  
- **Caching:** Redis (for session storage & caching queries)  
- **Containerization & Deployment:** Docker, Kubernetes, DigitalOcean/AWS  
- **CI/CD:** GitHub Actions / Jenkins  
- **Testing:** Postman, Jest / Pytest  
- **API Documentation:** Swagger / OpenAPI  

---

### Database Design
#### Users
- `userId`  
- `userName`  
- `email`  
- `phoneNumber`  
- `propertiesId[]`  
- `createdDate`  
- `updatedDate`

#### Properties
- `propertyId`  
- `location`  
- `userId`  
- `createdDate`  
- `updatedDate`

#### Bookings
- `bookingId`  
- `propertyId`  
- `userId`  
- `createdDate`  
- `updatedDate`

#### Reviews
- `reviewId`  
- `userId`  
- `propertyId`  
- `reviewMessage`  
- `createdDate`  
- `updatedDate`

#### Payment
- `paymentId`  
- `userId`  
- `bookingId`  
- `status`
- `createdDate`  
- `updatedDate`

---

### Team Roles
#### DevOps Engineer
Responsible for the **deployment of the backend system and database** to the cloud.

#### Backend Engineer
Manages the **system logic**, designs and codes the **core functionalities** of the application.

#### QA Engineer
Ensures the application meets **functional and non-functional requirements** through **testing and validation**.

#### Database Administrator
Designs and manages the **database schema, performance tuning, and optimizations**.

---

### Feature Breakdown
1. #### API Documentation
   - Provides navigation and usage of the REST APIs.

2. #### User Authentication
   - Manages user profiles.  
   - You can **get, create, update, and delete** the user’s profile.  

3. #### Property Management
   - Manages property details.  
   - You can **get, create, update, and delete** properties.  

4. #### Booking System
   - Manages property bookings.  
   - You can **get, create, update, and delete** booking arrangements.  

5. #### Payment Processing
   - Manages user payments and transactions.  
   - You can **initiate payments, verify transactions, process refunds, and view payment history**.  

6. #### Review System
   - Manages reviews and ratings for properties.  
   - Users can **add, edit, delete, and fetch reviews**.  
   - Supports **average rating calculations** per property.  

7. #### Database Optimizations
   - Ensures the system is **fast, scalable, and reliable**.  
   - Includes:  
     - Indexing for frequent queries  
     - Caching (e.g., Redis) for repeated requests  
     - Partitioning/Sharding for large datasets  
     - Connection pooling to handle traffic efficiently  

---

### API Security
- **JWT Authentication** for secure user sessions.  
- **Role-based access control (RBAC)** for different user permissions.  
- **Input validation & sanitization** to prevent SQL Injection/XSS.  
- **HTTPS/SSL** for encrypted communication.  

---

### CI/CD Pipeline
- **Continuous Integration (CI):**  
  - Runs automated tests (unit, integration).  
  - Code linting and formatting checks.  

- **Continuous Delivery/Deployment (CD):**  
  - Deploys Dockerized application to **cloud environments**.  
  - Supports **zero-downtime deployments**.  
  - Rollback mechanism in case of failure.