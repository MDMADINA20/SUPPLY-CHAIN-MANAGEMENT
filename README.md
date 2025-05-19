Here's a detailed breakdown of Supply Chain Management System Python program:

✅ Features of the Program
1)Inventory Management

2)View current stock levels.

3)Add stock (Restock feature).

4)Reduce stock when orders are placed.

5)Order Placement

6)Place orders for specific products and quantities.
7)Automatically updates inventory levels.
8)Displays order status: Fulfilled (if enough stock) or Backordered (if stock is insufficient).
9)Maintains and displays a history of all orders.
10)Supplier Management
11)Add suppliers along with the products they supply.
12)Display a list of all added suppliers.
13)Export Orders
14)Export order history to a CSV file.
15)User Interface
16)Graphical User Interface (GUI) built using tkinter.
17)Organized layout with labeled sections for each functionality.

🛠️ Technologies Used
Technology	Purpose:
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
