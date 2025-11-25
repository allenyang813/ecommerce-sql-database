# E-Commerce SQL Database & Trigger Implementation

## Overview
This project involved designing a complete SQL database for an e-commerce platform. It includes a relational schema covering users, products, orders, payments, loyalty points, gift cards, and returns. The project also required creating and testing triggers to enforce business rules for automated refund processing.

## What I Did
- Built a normalised relational database with entities such as:
  - Users, addresses, loyalty tracking
  - Products, orders, and order items
  - Payments, payment methods, and Afterpay instalments
  - Gift cards, returns, and refund records
- Inserted realistic sample data to model real e-commerce behaviour.
- Developed SQL triggers to automate refund workflows:
  - Forced all new ReturnedItem records to start with `Pending`.
  - Processed refunds only when a return switches to `Accepted`.
  - Calculated refund limits and selected the latest valid payment method.
  - Prevented invalid or declined returns from creating refund records.
- Tested triggers across multiple scenarios, including multi-payment orders and invalid inputs.

## Technologies Used
- SQL (MySQL)
- Relational database modelling
- Triggers, constraints, and automated business logic
- Data integrity, referential constraints, and transactional logic
