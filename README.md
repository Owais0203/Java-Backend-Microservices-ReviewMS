﻿# Java-Backend-Microservices-ReviewMS

Review Microservice
Overview
The Review Microservice manages reviews and ratings within my platform, providing functionalities to create, update, retrieve, and delete reviews for companies or other entities. It serves as a crucial component for gathering feedback and insights from users.

Features
Review CRUD Operations: Create, read, update, and delete operations for managing reviews.
Review Details: Store and retrieve details such as reviewer ID, reviewed entity ID (e.g., company), rating, and description.
Integration: Seamlessly integrates with other microservices, such as Company and User microservices, to provide comprehensive review-related functionalities.
Aggregate Ratings: Display aggregate ratings based on individual reviews for entities.

Dependencies
Database: Utilizes PostgreSQL database for storing review data.
Docker: Postgres container used for database

Endpoints
GET /reviews: Retrieve a list of all reviews.
GET /reviews/{reviewId}: Retrieve details of a specific review by ID.
POST /reviews: Create a new review.
PUT /reviews/{reviewId}: Update an existing review.
DELETE /reviews/{reviewId}: Delete a review by ID.
GET /reviews/entity/{entityId}: Retrieve all reviews for a specific entity (e.g., company).

