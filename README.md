# Project Proposal: DineSmart

## Overview

DineSmart is a comprehensive restaurant management system designed to streamline operations and enhance customer experience. It consists of a web application for diners to view the menu and place orders, a web application for managers to manage the menu and track orders, and a server to handle all backend operations.

### Problem

The restaurant industry faces challenges such as high labor costs and inefficiencies in order management. Customers often experience long wait times and lack of personalized service. Managers struggle with tracking popular menu items and overall operational efficiency. DineSmart addresses these issues by automating menu management and providing a seamless ordering experience for customers.

### User Profile

Customers

- Individuals dining at the restaurant who want a quick and easy way to view the menu and place orders.
- Accessed via a web application on their smartphones or tablets.

Managers

- Restaurant managers who need to manage the menu and track orders efficiently.
- Accessed via a web application on their desktop or laptop.

### Features

Diner Web Application:

- Browse Menu: View available food items categorized by type.
- Place Orders: Select items and place orders.

Manager Web Application:

- Manage Menu:
  - Add Food Type: Add new categories of food.
  - Add Food Item: Add new food items to the menu.
  - Edit Food Item: Modify details of existing food items.
  - Delete Food Item: Remove food items from the menu.
- Track Orders: View and manage current orders.

## Implementation

### Tech Stack

- Front-End Web Application: React, HTML, SASS, JavaScript
- Back-End: Express.js
- Database: MySQL
- Libraries and Tools: Bootstrap, WebSockets for real-time communication

### APIs

- Custom APIs developed using Express.js for handling menu and order data.

### Sitemap

Diner Web Application:

1. Menu Page: Browse menu items categorized by type.
2. Order Page: View cart and place orders.

Manager Web Application:

1. Menu: Overview of menu management.
2. Menu Management: Add, edit, and delete food types and items.
3. Order Tracking: Monitor and manage current orders.

### Mockups

Diner Web Application:

![Diner Web Application](https://github.com/chinghang0504/dine-smart/blob/main/Diner.PNG?raw=true)

Manager Web Application:

![Manager Web Application](https://github.com/chinghang0504/dine-smart/blob/main/Manager.PNG?raw=true)

### Data

- food_types (Table)
  - id
  - type
  - image
  - priority
- food_items (Table)
  - id
  - name
  - description
  - price
  - image
  - priority
  - type

### Endpoints

Diner Web Application:

- GET /menu/diner/foodtypes: Get all the food types
- GET /menu/diner/fooditems: Get the food items of a specific type

Manager Web Application:

- GET /menu/manager/foodtypes: Get all the food types
- POST /menu/manager/foodtypes: Create a new food type
- DELETE /menu/manager/foodtypes: Delete a food type
- PUT /menu/manager/foodtypes: Modify a food type
- GET /menu/manager/fooditems: Get all the food items
- POST /menu/manager/fooditems: Create a new food item
- DELETE /menu/manager/fooditems: Delete a food item
- PUT /menu/manager/fooditems: Modify a food item

## Roadmap

### Stage 1: Menu System (Creation)

- Diners can view the menu on their mobile devices.
- Display food categories, list of food items, and descriptions.

### Stage 2: Menu System (Improvement) [Before Deadline]

- Managers can manage the menu.
- Add items
- Edit item details
- Change item status
- Delete items

### Stage 3: Order System (Creation) [Before Demo day]

- Diners can modify their carts and place orders.
- Managers can receive and manage food orders.

## Nice-to-haves

- Advanced Analytics: Detailed insights such as customer behavior patterns.
- Loyalty Program: Implement a loyalty program for frequent customers.
- Multi-language Support: Support for multiple languages.
- Inventory Management: Track ingredient usage and alert when restocking is needed.
- Customer Feedback Integration: Allow customers to leave feedback directly through the app.

## Additionals

### GitHub Repository

- Project Proposal: https://github.com/chinghang0504/dine-smart
- Diner Web Application: https://github.com/chinghang0504/dine-smart-diner
- Manager Web Application: https://github.com/chinghang0504/dine-smart-manager
- Server Application: https://github.com/chinghang0504/dine-smart-server

### Instructions

- Read the README.md file in Server Application to setup the database and server.
- Read the README.md file in Manager Web Application to setup.
- Read the README.md file in Diner Web Application to setup.

### References

- Sushi California: https://sushi-california.com/
