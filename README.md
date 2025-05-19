Features
Inventory Management

Shows a list of products and their quantities.
Allows restocking items (adding more stock to inventory).
Real-time inventory updates after orders/restocking.
Order Placement

Users can place orders for any listed product.
Checks if enough stock is available to fulfill the order.
Marks orders as “Fulfilled” or “Backordered” based on stock availability.
Keeps a timestamped history of all orders.
Supplier Management

Add new suppliers and the products they supply.
Displays a list of all suppliers added during the session.
Order History

Shows a table of all orders placed with time, product, quantity, and status.
Allows exporting the order history to a CSV file.
Technologies Used
Python: The programming language used to write the entire program.
tkinter: Python’s standard GUI (Graphical User Interface) library for building desktop applications.
ttk: Themed tkinter widgets for a modern look (used for tables, dropdowns, etc.).
csv: Python’s built-in module for reading and writing CSV (Comma-Separated Values) files (used for exporting orders).
datetime: For generating readable timestamps for orders.
How It Works
Initialization

The program defines two main classes: Inventory (for managing stock) and SupplyChainApp (handles all GUI and logic).
Predefined inventory items and quantities are set up when the app starts.
User Interface

The main window displays sections for Inventory, Placing Orders, Restocking, Supplier Management, and Order History—all with interactive widgets.
Inventory and orders are shown in tables (using ttk.Treeview).
Order Placement

The user selects a product and quantity and submits an order.
If enough stock exists, inventory is reduced, and the order is marked "Fulfilled"; if not, it’s "Backordered."
Orders are added to the history with a timestamp.
Restocking

The user can select a product and enter a quantity to add to the inventory.
Inventory is updated immediately.
Supplier Management

Users can add new suppliers and products they supply.
Supplier entries are shown in a list.
Order Export

The user can export the order history to a CSV file for external record-keeping.
In short:

The application is a GUI-based supply chain management tool built in Python, using tkinter for the interface and some standard libraries for data handling.
It supports inventory tracking, order management, supplier tracking, and data export, all through a user-friendly interface.
