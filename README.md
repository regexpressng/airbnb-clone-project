# airbnb-clone-project

## Brief overview of the project

- ### Goals

- ### Technology Stack

  ### Database Design
  - #### Users
    - userId
    - userName
    - email
    - phoneNumber
    - propertiesId[]
    - createdDate
    - updatedDate

  - #### Properties
    - propertyId
    - propertyId
    - location
    - userId
    - createdDate
    - updatedDate

  - #### Bookings
    - bookingsId
    - propertyId
    - userId
    - createdDate
    - updatedDate

  - #### Reviews
    - userId
    - propertyId
    - reviewId
    - reviewMessage
    - createdDate
    - updatedDate

  - #### Payment
    - paymentId
    - Userid
    - Bookingsid
    - createdDate
    - updatedDate


- ### Team Roles
    - #### DevOps Engineer
        - The Devops engineer would be responsible for the deployment of the backend system and database to the cloud.

    - #### Backend Engineer
        - The Backend engineer manages the system logic, they design and code the core functionalities of the application.

    - #### QA Engineer
        - The QA checks and ensures that the application meets the requirements required of it. Both the functional and non-functional requirements

    - #### Database Administrator
        - The Database administrator designs and manages the database.


- ### Feature Breakdown
    1. #### API Documentation
        - This helps with the documentation and navigation of the rest api's

    2. #### User Authentication
        - The user Authentication is the api that manages user profiles, You can get, create, update and delete the user's profile.

    3. #### Property Management
        - The Property Management is the api that manages property details, You can get, create, update and delete the property.

    4. #### Booking System
         - The Booking System API manages property bookings.
         - You can get, create, update, and delete booking arrangements.

    5. #### Payment Processing
        - The Payment Processing API manages user payments and transactions.
        - You can initiate payments, verify transactions, process refunds, and view payment history.

    6. #### Review System
        - The Review System API manages reviews and ratings for properties.
        - Users can add, edit, delete, and fetch reviews.
        - Supports average rating calculations per property.

    7. #### Database Optimizations

        - Ensures the system is fast, scalable, and reliable.
        - Includes:
            - Indexing for frequent queries
            - Caching (e.g., Redis) for repeated requests
            - Partitioning/Sharding for large datasets
            - Connection pooling to handle traffic efficiently
    
- ### API Security

- ### CI/CD Pipeline