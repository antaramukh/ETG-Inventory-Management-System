# ETG_Inventory_Management_System

The Inventory System Management Project consists of 4 files:

1. Inventory Management System - Record.ipynb
2. record.json
3. Inventory Management System - Sales.ipynb
4. sales.json

The "Inventory Management System - Record.ipynb" file deals with the management and functionalities to do with the "record.json" file.

1. The json.loads() method converts JSON into a dict object and it is stored in the variable "product".
2. Each product has 5 attributes: product_name, retail_price, discounted_price, category, qty.
3. New products can be added by asking the user to input the Product ID, Product Name, MRP, Discounted price, Category and Quantity. 
4. The already existing products can be edited/updated by asking the user for the Product ID and asking them to choose the attribute they would like to change.
5. The existing products can be deleted by asking the user for Product ID.
6. After each functionality is performed, the updated values of the "product" dict are updated in the inventory "record.json" using json.dumps() function.

The "Inventory Management System - Sales.ipynb" file deals with the management and functionalities to do with the "sales.json" file.

1. First, the inventory is read from the "record.json" file and the json.loads() method converts JSON into a dict object and it is stored in the variable "product".
2. Each product has 5 attributes: product_name, retail_price, discounted_price, category, qty.
3. The customer is then asked which product they would like to purchase by asking them for the Product ID and Quantity of the product.
4. A bill is generated which displays the Product Name, Quantity, Price of each product and the Total Bill to be paid.
5. After the purchase, the updated values of the "product" dict are updated in the inventory "record.json" using json.dumps() function.
6. Then, the "sales.json" file is read using the json.loads() method and converting the JSON into a dict object and storing in the variable "sales".
7. The sales dict has 5 attributes: "product_id", "prod_name", "qty", "amount", "time_of_purchase".
8. The sale that was made is updated in the "sales" dict.
9. The updated values of the "sales" dict are updated in the "sales.json" using json.dumps() function.

