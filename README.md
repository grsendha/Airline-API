# ✈️Airline-API
- This project is a microservice-based architecture designed to manage various functionalities of an airline booking system. The system is composed of several independent services that communicate with each other, each handling a specific aspect of the overall application. Below is a detailed description of each microservice included in this project.

## 🤖tech Stack
- Node.js: JavaScript runtime for server-side development
- Express.js: Web application framework for Node.js
- Body-parser: Middleware for parsing incoming request bodies
- Sequelize: Promise-based Node.js ORM for relational databases
- dotenv: Module for loading environment variables

## 🔗 [FlightAndSearchService](https://github.com/grsendha/FlightAndSearchService)  

This micro-service mainly focuses on creation, deletion, updation and fetching of all the flights, airports and cities in the database. The APIs which read the flights from databases are exposed to the customers, others can only be accessed by the Admins.

- Provides the user with the flexibility to query about the flights-
    - User can select the number of seats,class of flight .
    - Support filters of flights based on Price, Departure time,Duration. .

## 🔗 [AuthService](https://github.com/grsendha/AuthService)  

This micro-service mainly focuses on the authorization and authentication of the users.

- Authentication: It is a process by which we can uniquely identify users on our application. This process tells about who the user is.

- Authorization: It is a process by which we can identify the capabilities of a user i.e what a user can do in our application. Eg, we use Flipkart so when logging in as a normal user you have different access and when you log in as a seller it's different, a seller can sell the products on the app, not the normal user.


## 🔗 [ReminderService](https://github.com/grsendha/ReminderService)  

- This repository contains the code for an email reminder service built using Node.js and Express. The service is designed to send email reminders at specified times.
  ### Tech Stack
  - Nodemailer: Module for sending emails with Node.js
  - Cron: Library for scheduling tasks in Node.js
  - AMQP (RabbitMQ): Message broker for handling message queues

## 🔗 [BookingService](https://github.com/grsendha/BookingService)  

The BookingService handles all aspects of the booking process. Key features include:
- **Flight Reservations**: Manages the booking of flights, including seat selection and payment processing.
- **Booking Management**: Provides endpoints for users to view, modify, or cancel their bookings.


## 🔗 [APIGateway](https://github.com/grsendha/APIGateway)  

- We need an intermediate layer between the client side and the microservices
- Using this middle end , when client sends request we will be able to make decision that which microservice should actually respond to this request
- We can do message validation, response transformation , rate limiting
- We try to prepare an API Gateway that acts as this middle end



