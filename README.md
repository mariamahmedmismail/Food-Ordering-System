Food Ordering System – Project Implementation
📌 Overview

This project is a Food Ordering System that allows customers to register, manage their accounts, place orders, give feedback, and interact with the menu. The database is designed with multiple entities including Customer, Order, Menu, Meal, Feedback, and Restaurant.

This README explains the implemented functionalities for Customer and Feedback tables, focusing on insertion, deletion, and update operations with proper validation.

🛠 Implemented Features

1️⃣ Customer Table Operations
🔹 Insert (Sign Up)

Before inserting a new customer record, the system checks if:

The email already exists in the Customer table.

If it exists, sign-up is blocked with a message:

"This email is already registered. Please log in."

If not, the customer details are added successfully.

🔹 Update (Profile Update)

The customer must provide their correct registered email.

If the email exists in the database:

The update is applied (e.g., name, phone, address).

If not:

The update fails with a message:

"Invalid email. Update not allowed."

🔹 Delete (Account Removal)

Customers cannot delete their account without providing their correct email.

The system checks if the provided email exists in Customer.

If it exists, deletion is executed; otherwise, an error message is returned.

2️⃣ Feedback Table Operations
🔹 Insert (Add Feedback)

Customers can add feedback for a meal if:

Their email exists in Customer.

The Meal_ID exists in the Meal table.

🔹 Update (Edit Feedback)

The customer must provide:

Correct email (validated against Customer table).

Correct meal ID (validated against Meal table).

If validation passes, the feedback is updated. Otherwise, an error is displayed.

🔹 Delete (Remove Feedback)

A feedback record can only be deleted by the customer who created it.

Email verification is required.

💻 Tech Stack

Database: MySQL 

Backend: SQL + C#

Entities: Customer, Order, Menu, Meal, Feedback, Restaurant, Payment
