# LogisticsAnalytics

Schema

Warehouses:

warehouse_id INT PRIMARY KEY,
warehouse_name VARCHAR(255),
location VARCHAR(255),
capacity DECIMAL(10, 2)

Products 
product_id INT PRIMARY KEY,
product_name VARCHAR(255),
category VARCHAR(100),
price DECIMAL(10, 2)

Shipments 
shipment_id INT PRIMARY KEY,
product_id INT,
warehouse_id INT,
quantity INT,
shipment_date DATE,

Orders:
order_id INT PRIMARY KEY,
product_id INT,
customer_name VARCHAR(255),
order_date DATE,
quantity INT,
shipping_address VARCHAR(500)
