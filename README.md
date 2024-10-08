﻿# pharma-drugs-shop

Here's a detailed note for your GitHub README file for a Pharma & Drugs Supplier Management System:

---

# Pharma & Drugs Supplier Management System

This project is a comprehensive Pharma & Drugs Supplier Management System built using Python and SQLite3. The application helps pharmaceutical companies and suppliers manage their drug inventory, suppliers, and orders efficiently. It includes features for adding, editing, deleting, and viewing drug and supplier information, along with tracking orders and inventory levels.

## Features

### 1. **Drug Management**
   - **Add Drug**: Allows users to add new drugs to the inventory with details such as:
     - **Drug Name**: The name of the drug.
     - **Batch Number**: Unique identifier for the drug batch.
     - **Expiration Date**: Date when the drug expires.
     - **Quantity**: Number of units available in stock.
     - **Price**: Cost per unit.
     - **Supplier**: The supplier providing the drug.
   - **Edit Drug**: Users can update existing drug details such as quantity, price, or expiration date.
   - **Delete Drug**: Allows users to remove drugs from the inventory.
   - **View Drugs**: Displays a list of all drugs in the inventory with their details, including search and filter functionality.

### 2. **Supplier Management**
   - **Add Supplier**: Users can add new suppliers with details such as:
     - **Supplier Name**: The name of the supplier.
     - **Contact Person**: The primary contact person at the supplier.
     - **Phone Number**: Contact number for the supplier.
     - **Email**: Email address for communication.
     - **Address**: Physical address of the supplier.
   - **Edit Supplier**: Users can update supplier information, such as contact details or address.
   - **Delete Supplier**: Allows users to remove a supplier from the system.
   - **View Suppliers**: Displays a list of all suppliers with their details, including search and filter functionality.

### 3. **Order Management**
   - **Create Order**: Users can create new orders to request drugs from suppliers. This includes:
     - **Order Date**: The date the order is placed.
     - **Drug Details**: List of drugs being ordered, along with quantities.
     - **Supplier**: The supplier from whom the order is placed.
     - **Order Status**: Track the order status (e.g., Pending, Completed, Cancelled).
   - **Edit Order**: Update order details, such as quantities or status.
   - **Delete Order**: Remove orders from the system.
   - **View Orders**: Display all orders with details such as drug names, quantities, supplier, and status.

### 4. **Inventory Management**
   - **Stock Levels**: Automatically update inventory levels based on orders placed and received.
   - **Low Stock Alerts**: Notify users when drug quantities fall below a predefined threshold.
   - **Expiration Alerts**: Notify users when drugs are nearing their expiration date.

### 5. **Reports and Analytics**
   - **Inventory Reports**: Generate reports on current stock levels, low stock items, and expired drugs.
   - **Order Reports**: Generate reports on orders placed, completed, and pending.
   - **Supplier Reports**: Generate reports on supplier performance, including order fulfillment rates and delivery times.
   - **Sales Reports**: Track sales data, including total revenue and top-selling drugs.

### 6. **User Management (Optional)**
   - **Admin Users**: Manage all aspects of the system, including drugs, suppliers, and orders.
   - **Regular Users**: Limited access, such as viewing inventory and creating orders.

### 7. **Security Features**
   - **Authentication**: Secure login for users with role-based access control (Admin, User).
   - **Data Encryption**: Encrypt sensitive data in the database, such as passwords.
   - **Backup & Restore**: Regular database backups and restore functionality to prevent data loss.

### 8. **Responsive Design (Optional)**
   - **GUI (Optional)**: A graphical user interface using Tkinter or any web framework to interact with the application.
   - **Command Line Interface**: For users who prefer interacting via the terminal.

## Technologies Used

- **Python**: The primary programming language used for application logic.
- **SQLite3**: A lightweight, file-based database for storing drug, supplier, and order information.
- **Optional GUI**: Tkinter for a simple graphical interface or Flask/Django for a web-based interface.

## Prerequisites

Ensure you have Python installed on your system. SQLite3 is included with Python by default.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/pankajkr-143/pharma-drugs-shop/.git
   ```
2. Navigate to the project directory:
   ```bash
   cd pharma-drugs-shop
   ```
3. Install any required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
   *(Note: If you're using a GUI framework like Flask or Django, include those in `requirements.txt`.)*

## Usage

1. **Run the Application**:
   - If using a command-line interface:
     ```bash
     python app.py
     ```
   - If using a GUI or web interface:
     ```bash
     python app_gui.py  # or app_web.py depending on the implementation
     ```

2. **Adding Drugs and Suppliers**:
   - Enter details for new drugs and suppliers via the add forms.

3. **Managing Orders**:
   - Create new orders, update existing ones, and track order status.

4. **Viewing and Editing Data**:
   - Browse and update existing drugs, suppliers, and orders through the respective views.

5. **Generating Reports**:
   - Use the reporting feature to generate detailed reports on inventory, orders, and supplier performance.

## Database Structure

- **Database**: `pharma.db`
- **Tables**:
  - **Drugs**:
    - **ID**: Primary key, auto-incremented.
    - **Name**: Text.
    - **Batch Number**: Text.
    - **Expiration Date**: Date.
    - **Quantity**: Integer.
    - **Price**: Real.
    - **Supplier**: Foreign key linking to suppliers.
  - **Suppliers**:
    - **ID**: Primary key, auto-incremented.
    - **Name**: Text.
    - **Contact Person**: Text.
    - **Phone Number**: Text.
    - **Email**: Text.
    - **Address**: Text.
  - **Orders**:
    - **ID**: Primary key, auto-incremented.
    - **Order Date**: Date.
    - **Supplier**: Foreign key linking to suppliers.
    - **Status**: Text (e.g., Pending, Completed, Cancelled).

## Example

1. **Add a Drug**:
   - Drug Name: "Paracetamol"
   - Batch Number: "B12345"
   - Expiration Date: "2025-12-31"
   - Quantity: 1000
   - Price: 1.50
   - Supplier: "ABC Pharma"

2. **Create an Order**:
   - Order Date: "2024-08-10"
   - Supplier: "ABC Pharma"
   - Drugs Ordered: "Paracetamol (500 units)"
   - Status: "Pending"

3. **View Reports**:
   - Generate a report showing low stock items and upcoming expirations.

## Contributing

Contributions are welcome! Fork this repository, create a new branch, and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

This README note outlines the features, usage, and technical details of your Pharma & Drugs Supplier Management System, providing clear guidance on how to use and contribute to the project.
