🧳 ALX Travel App 0x00
A backend service designed for managing travel listings, bookings, and guest reviews — built as part of the ALX Backend learning curriculum.

This project includes:

Cleanly defined Django models

RESTful API serializers

A custom command to quickly seed the database with sample data for development/testing

 Features
 Listings Management
Create and store travel property listings with location, price, and descriptions. Perfect for showcasing getaways!

 Bookings
Allow guests to book listings with check-in and check-out dates, and track booking status.

 Guest Reviews
Guests can leave a review and rating for completed bookings, supporting quality feedback.

Database Seeding
A Django management command to populate the database with mock listings, bookings, and reviews for quick testing.

Project Structure
(Basic Django project layout with apps for Listings, Bookings, and Reviews — details omitted for brevity)

️ Models Overview
 Listing
host (ForeignKey → User)

title, description, location

price_per_night

created_at, updated_at timestamps

 Booking
listing (ForeignKey → Listing)

guest (ForeignKey → User)

check_in, check_out, status

 Review
booking (OneToOneField → Booking)

reviewer (ForeignKey → User)

rating, comment

 Serializers
ListingSerializer – Handles data representation for listings

BookingSerializer – Manages booking data for the API

️ Usage
Clone the repo

Run migrations

Use the seed command to generate sample data

Start the development server

Access the API endpoints and explore the app!


