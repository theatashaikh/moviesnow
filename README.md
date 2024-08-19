## MovieNow: An Online Movie Rental Company

### Overview
Introduction to MovieNow, a fictional movie rental company with a Postgres database. Customers can rent movies for 24 hours. The company stores information about movies, customers, and ratings.

### MovieNow Data Structure

- **Movies Table**
  - `movie_id`: Unique identifier
  - `title`, `genre`, `runtime`, `release_year`, `rental_cost`

- **Actors Table**
  - `actor_id`: Unique identifier
  - `name`, `year_of_birth`, `nationality`, `gender`

- **Actsin Table**  
The actsin table stores information regarding which actor acted in which movies.
  - `actsin_id`: Unique identifier
  - `movie_id`, `actor_id`

    
- **Customers Table**
  - `customer_id`: Unique identifier
  - `name`, `country`, `gender`, `date_of_birth`, `account_creation_date`

- **Renting Table**  
The renting table stores information regarding which customer rented which movie on which date and after watching the movie what rating the customer gave. rating from 1-10 where 10 is the best.
  - `renting_id`: Unique identifier
  - `customer_id`, `movie_id`, `rating`, `rental_date`

### Objectives of Data-Driven Decision-Making
-  Data-driven decisions support short-term and long-term goals. Examples include:
  - Short-term: Popularity of actors, last month's revenue.
  - Long-term: Customer growth, regional successes, overall revenue trends.

### Key Performance Indicators (KPIs)
- KPIs help monitor success. Examples for MovieNow:
  - **Revenue**: Sum of rental prices.
  - **Customer Satisfaction**: Average movie rating.
  - **Customer Engagement**: Number of active customers over time.
