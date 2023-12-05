# Restaurants--without-SQLAlchemy

This Python script implements a simple restaurant review system with classes representing customers, restaurants,
and reviews. Customers can leave reviews for restaurants, and restaurants can be reviewed by multiple customers.
The system also provides functionality to retrieve information such as customer and restaurant details, average
star ratings for restaurants, and more.

# Classes

**Customer**
Attributes
given_name: First name of the customer.
family_name: Last name of the customer.
reviews: List of reviews left by the customer.

**Methods**
full_name(): Returns the full name of the customer.
restaurants(): Returns a list of restaurants reviewed by the customer.
add_review(restaurant, rating): Adds a new review for a restaurant.
num_reviews(): Returns the number of reviews left by the customer.

**Class Methods**
all(): Returns a list of all customer instances.
find_by_name(name): Finds a customer by full name (case-insensitive).
find_all_by_given_name(name): Finds all customers with a given first name (case-insensitive).

# Restaurant

**Attributes**
name: Name of the restaurant.
reviews: List of reviews received by the restaurant.

**Methods**
reviews(): Returns a list of reviews received by the restaurant.
customers(): Returns a list of customers who reviewed the restaurant.
average_star_rating(): Calculates and returns the average star rating for the restaurant.

**Class Methods**
all(): Returns a list of all restaurant instances.

# Review

**Attributes**
customer: The customer who left the review.
restaurant: The restaurant that is reviewed.
rating: The star rating given in the review.

**Methods**
customer(): Returns the customer who left the review.
restaurant(): Returns the restaurant that is reviewed.
rating(): Returns the star rating given in the review.

**Class Methods**
all(): Returns a list of all review instances.
