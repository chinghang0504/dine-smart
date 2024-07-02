# Project Title

DineSmart

## Overview

DineSmart is a comprehensive restaurant management system designed to streamline operations, enhance customer experience, and provide valuable insights for managers. It includes a web application for customers to order food and receive AI-based recommendations, a mobile application for employees to check order statuses, and a desktop application for managers to analyze order history, manage menu items, and performance.

### Problem

The restaurant industry faces significant challenges such as high labor costs, inefficiencies in order management, and the need for timely and accurate food recommendations. Customers often experience long wait times and lack personalized recommendations, while managers struggle with tracking popular menu items and overall operational efficiency. DineSmart aims to address these pain points by automating order processes, providing AI-driven food recommendations, and offering robust analytics for better decision-making.

### User Profile

Customers

- Individuals dining at the restaurant who want a quick and easy way to order food and receive personalized recommendations.
- Via a web application accessible on their smartphones or tablets to place orders and receive AI recommendations.

Employees

- Restaurant staff who need to track and manage food orders efficiently.
- Through a mobile application on tablets or smartphones to monitor and update the status of food orders.

Managers

- Restaurant managers who require detailed insights into order history, the ability to manage menu items, and overall performance.
- Using a desktop application to review order history, analyze trends, manage menu items, and generate reports.

### Features

Customer Web Application:

- Browse menu items and place orders.
- Receive AI-based food recommendations.
- Track order status in real-time.

Employee Mobile Application:

- View incoming orders and their status.
- Update order status (e.g., preparing, ready for pickup).
- Receive notifications for new orders.

Manager Desktop Application:

- Access order history and detailed reports.
- Analyze popular and least popular menu items.
- Monitor real-time order status and kitchen performance.
- Login to the server to add or remove food items from the menu.

## Implementation

### Tech Stack

- Front-End Web Application: React, HTML, SASS, TypeScript
- Front-End Mobile Application: Android (Kotlin)
- Back-End: Spring Boot (Java)
- Data Analysis: Python, NumPy, Pandas, Matplotlib
- Database: MySQL
- Artificial Intelligence: OpenAI GPT-4
- Libraries and Tools: Material-UI, WebSockets for real-time communication

### APIs

- OpenAI GPT-4 API: For AI-based food recommendations.

### Sitemap

Web Application (Customer):

- Home Page: Browse menu and place orders.
- Order Status: Track order status.
- Recommendations: View AI-based food recommendations.

Mobile Application (Employee):

- Order Dashboard: View and manage current orders.
- Notifications: Receive real-time updates on new orders.

Desktop Application (Manager):

- Dashboard: Overview of order statuses and performance.
- Order History: Detailed reports and analytics on past orders.
- Analytics: Visualizations of popular menu items and trends.
- Menu Management: Add or remove food items from the menu.

### Mockups

Web Application (Customer):

- Not implemented yet.

Mobile Application (Employee):

- Not implemented yet.

Desktop Application (Manager):

- Not implemented yet.

### Data

- Account: accountID, accountType, username, password
- MenuItem: menuItemID, name, description, price, category
- Order: orderID, tableID, menuItemIDs, status, timestamp

### Endpoints

Web Application (Customer):

- GET /menu (Get all the menu items)
- POST /order (Send a food order)
- GET /recommendation (Get AI-based food recommendations)

Mobile Application (Employee):

- GET /orders (Get list of all current orders)
- PUT /orders/:id (Update order status)

Desktop Application (Manager):

- GET /orders/history (Get order history)
- POST /menuitem (Add a new menu item)
- DELETE /menuitem/:id (Delete a menu item)

### Auth

- Authentication: Use JWT (JSON Web Tokens) for user login and registration.
- Authorization: Role-based access control to ensure that customers, employees, and managers have appropriate access to features. Only the manager can change the menu items.

## Roadmap

### Stage 1: Menu System (Creation)

#### Objectives:

- Allow diners to view the menu on their mobile devices.

#### Features:

1. Food Category View:
   - Display various categories of food available.
2. List of Food Items:
   - Show the list of food items under each category.
3. Food Description:
   - Provide detailed descriptions of each food item including ingredients, price, and images.

### Stage 2: Menu System (Improvement)

#### Objectives:

- Enable managers to manage the menu items.

#### Features:

1. Add Items:
   - Managers can add new items to the menu.
2. Change Item Details:
   - Managers can update details of existing items (e.g., price, description).
3. Change Item Status:
   - Managers can change the status of menu items (e.g., available, out of stock).
4. Delete Items:
   - Managers can remove items from the menu.
5. Database Storage:
   - All menu items are stored in a database.
6. Cache System:
   - Implement a caching system to efficiently retrieve menu items.

### Stage 3: Order System (Creation)

#### Objectives:

- Allow diners to modify their carts and send orders. Enable managers to receive orders.

#### Features:

1. Modify Cart:
   - Diners can add items to their cart.
   - Diners can delete items from their cart.
2. Send Orders:
   - Diners can place their food orders through the app.
3. Receive Orders:
   - Managers can receive and view food orders in real-time.

### Stage 4: Auth System (Creation)

#### Objectives:

- Implement an authentication system to manage user roles.

#### Features:

1. Root Account:
   - The root account can create manager accounts.
2. Manager Account:
   - Manager accounts can modify the menu.
   - Manager accounts can receive food orders.

### Stage 5: Order System (Improvement)

#### Objectives:

- Enhance the order system to manage table identifications.

#### Features:

1. Table Identification:
   - Managers can select different table identifications.
   - Option to use fixed table IDs or generate unique table IDs for each order session.

## Nice-to-haves

- Advanced Analytics: More detailed insights such as customer behavior patterns.
- Loyalty Program: Implement a loyalty program for frequent customers.
- Multi-language Support: Support for multiple languages to cater to a diverse customer base.
- Inventory Management: Track ingredient usage and alert when restocking is needed.
- Customer Feedback Integration: Allow customers to leave feedback directly through the app and use this data to further refine AI recommendations.
