Here's a detailed breakdown of your Supply Chain Management System Python program:

✅ Features of the Program
1)Inventory Management

 i)View current stock levels.

 ii)Add stock (Restock feature).

 iii)Reduce stock when orders are placed.

2)Order Placement

 i)Place orders for specific products and quantities.

 ii)Automatically updates inventory levels.

 iii)Displays order status: Fulfilled (if enough stock) or Backordered (if stock is insufficient).

 iv)Maintains and displays a history of all orders.

3)Supplier Management

  i)Add suppliers along with the products they supply.

  ii)Display a list of all added suppliers.

4)Export Orders

  i)Export order history to a CSV file.

5)User Interface

  i)Graphical User Interface (GUI) built using tkinter.

  ii)Organized layout with labeled sections for each functionality.

🛠️ Technologies Used
Technology	Purpose
  1)Python	Main: programming language
  2)Tkinter:For creating the graphical user interface (GUI)
  3)ttk (Themed Widgets):For styled GUI components like Treeview, Combobox
  4)messagebox & filedialog:To show alerts and save file dialogs
  5)datetime:To timestamp orders
  6)csv:To export orders to a CSV file

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
