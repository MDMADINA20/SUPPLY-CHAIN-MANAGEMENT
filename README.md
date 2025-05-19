Here's a detailed breakdown of your Supply Chain Management System Python program:

✅ Features of the Program
Inventory Management

View current stock levels..

Add stock (Restock feature).

Reduce stock when orders are placed.

Order Placement

Place orders for specific products and quantities.

Automatically updates inventory levels.

Displays order status: Fulfilled (if enough stock) or Backordered (if stock is insufficient).

Maintains and displays a history of all orders.

Supplier Management

Add suppliers along with the products they supply.

Display a list of all added suppliers.

Export Orders

Export order history to a CSV file.

User Interface

Graphical User Interface (GUI) built using tkinter.

Organized layout with labeled sections for each functionality.

🛠️ Technologies Used
Technology	Purpose
Python	Main programming language
Tkinter	For creating the graphical user interface (GUI)
ttk (Themed Widgets)	For styled GUI components like Treeview, Combobox
messagebox & filedialog	To show alerts and save file dialogs
datetime	To timestamp orders
csv	To export orders to a CSV file

⚙️ How It Works (Logic and Flow)
Startup

run_supply_chain_app() creates the main window and initializes the app.

SupplyChainApp class sets up inventory, suppliers, orders, and GUI widgets.

Inventory System

Inventory class manages a dictionary of products and quantities.

Provides add_stock(), reduce_stock(), and get_stock() methods.

Placing Orders

User selects a product and enters quantity.

On submit:

The app checks if stock is enough.

Reduces stock if available.

Adds the order to history with time, product, quantity, and status.

Restocking Inventory

User selects a product and quantity to add.

Updates the inventory.

Managing Suppliers

User inputs a supplier name and the product they supply.

Adds this information to a list and displays it.

Order Export

User clicks “Export Orders to CSV”.

Opens file save dialog.

Writes all order data to a .csv file.
