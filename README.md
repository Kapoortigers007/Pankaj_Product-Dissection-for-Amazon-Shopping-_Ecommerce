# Pankaj_Product-Dissection-for-Amazon-Shopping-_Ecommerce

Capstone Project: Product Dissection for Amazon Shopping App

Company Overview:

Amazon was founded on July 5, 1994, by Jeff Bezos. Amazon’s headquarters are located in Seattle, Washington, USA. It is a technology and e-commerce company, and it is one of the largest online retailers in the world.
The Amazon shopping app is a mobile application that allows users to shop for a wide range of products, including electronics, books, clothing, and much more. Users can browse, search, and make purchases using the app.
Now, Amazon is also expanding its business to Amazon Pay, Amazon Cloud services, etc.


Product Dissection and Real-World Problems Solved by Amazon

Amazon, a worldwide e-commerce leader, has skilfully managed real-life challenges via its inventive product solutions. By prioritising the simplification of the online shopping journey, Amazon enables consumers to explore an extensive variety of products and services, connecting the divide between conventional retail and the ease of e-commerce. Amazon simplifies the challenge of contemporary shopping needs by offering a user-friendly platform for customers to search, buy, and track their orders, allowing individuals to effortlessly and quickly locate what they require.


Amazon's creative functions, including one-click purchasing, tailored product suggestions, and the use of consumer reviews, have changed the way people interact with e-commerce. By tackling the issue of decision-making in the online market, Amazon simplifies the buying process, aiding customers in making educated decisions. Additionally, Amazon's launch of Prime membership has transformed the idea of convenience by providing quick and dependable shipping, a vast selection of digital content, and unique discounts. This creative method successfully addresses the issue of efficiency and enhanced advantages, allowing users to confidently meet their shopping requirements with ease.

Summary: 

Amazon's product design has effectively addressed real-world challenges by developing a platform that streamlines online shopping, provides convenience, and satisfies the changing needs of consumers. With its wide range of features and services, Amazon fulfils the demand for effective e-commerce, informed choices, and improved customer satisfaction, transforming the digital retail environment and offering tangible solutions for a varied global audience
Case Study: Real-World Problems and Amazon's Innovative Solutions

Amazon is a leading Online shopping marketplace that has not only revolutionised the way we can buy and sell goods, but also how we share and consume content, and has also addressed significant real-world challenges through its innovative features. By identifying user needs and leveraging technology, Amazon has positioned itself as a solution-driven platform that fosters connections, encourages self-expression, and enhances digital interactions.


Amazon's notable attributes directly tackle practical issues, showcasing the platform's dedication to improving user experiences and delivering solutions that meet a variety of requirements. From optimising the buying process to guaranteeing fast and dependable delivery, aiding companies in expanding their operations, or linking sellers to an international marketplace, Amazon's functionalities significantly address real-world challenges for users and businesses alike


Problem 1: Convenience and Accessibility:
Real-World Challenge: Traditional shopping often requires physical presence, which can be time-consuming and less convenient.

Amazon's Solution: Amazon shopping allows users to shop for a wide range of products from the comfort of their homes or anywhere they have internet access. This convenience is especially valuable for people with busy schedules, mobility challenges, or those living in remote areas.
Problem 2: Wide Product Selection:
Real-World Challenge: Local stores may have limited product selections, making it challenging to find specific items.

Amazon's Solution:
The Amazon app provides access to an extensive catalogue of products, ranging from everyday essentials to niche items. This breadth of selection enables one to find and purchase a wide variety of products easily.
Problem 3: Secure Transactions:
Real-World Challenge: Concerns about the security of online transactions can deter some consumers from shopping online.

Amazon's Solution:
Amazon employs advanced security measures, including secure payment processing, data encryption, and buyer protection policies, to ensure that transactions are secure and protect user information.
Problem 4: Personalisation:
Real-World Challenge: Shoppers often want a more personalised shopping experience.

Amazon's Solution: Amazon’s app uses algorithms to provide personalised product recommendations based on a user’s browsing and purchase history, making it easier for users to discover new products of interest.
Conclusion:
In summary, the Amazon shopping app addresses various real-world problems by providing a convenient, accessible, and efficient platform for online shopping, offering a wide selection of products, facilitating price comparisons, ensuring reliable delivery, and incorporating user reviews and personalised recommendations to enhance the shopping experience for users. It also provides a secure payment facility.
Top Features of the Amazon Shopping App:

Product Search: We can use the search bar to look for products on Amazon by typing in keywords, product names, or even scanning barcodes. This feature makes it easy to find the specific items you’re looking for.

Product Details: When we select a product, we’ll see detailed information about it, including product descriptions, images, customer reviews, and pricing. This helps you make informed purchasing decisions.

One-Click Ordering: If one has saved their payment and shipping information, they can make purchases with just one click, which streamlines the checkout process and makes it faster and more convenient.

Wish List: You can create lists of products you’re interested in buying in the future. This helps you keep track of items you want, and you can even share your lists with others, like for gift ideas.

Track Orders: The app lets you keep tabs on the status of your orders. You can see when they’ve been shipped and receive notifications when they’re out for delivery or have been delivered.

Product Reviews: We can read and write reviews for products we have purchased, helping other shoppers make informed decisions. It’s a way for customers to share their experiences with a product.
Schema Description: 

The schema for Amazon involves multiple entities that represent different aspects of the platform. These entities include Customer, Order, Product, Shipment, Payment, Cart, and more. Each entity has specific attributes that describe its properties and relationships with other entities.

Customer Entity: Customers are at the core of Amazon. The customer entity contains information about each customer:

Customer_id (Primary Key): A unique identifier for each customer.
Full_name: The customer's full name is registered on the app.
Email: The customer's email address for account-related communication.
Address: Customer address to deliver the product to that address.
Phone_number: The customer’s contact number to contact that customer.

Product Entity:
Product entity contains information about all products:

Product_id (Primary Key): A unique identifier for each product.
Name: Name of the product.
Description: Details regarding the products.
Price: Price of the product.
Stock: Number of quantities.

Order Entity:
Customers place the order. We will store order details in the Order entity:

Order_id (Primary Key): A unique identifier for each order.
Customer_id (Foreign Key referencing Customer Entity): The customer who orders.
Product_id (Foreign Key referencing Product Entity): The product that has been ordered.
Shipment_id (Foreign Key referencing Shipment Entity): The order goes for shipment.
Payment_id (Foreign Key referencing Payment Entity): The Payment details for that order.
Order_date: The date when the customer orders.
Total_price: Price after discount and shipment charge.

Payment Entity:
Likes represent user appreciation for posts:

Payment_id (Primary Key): A unique identifier for each payment.
Customer_id (Foreign Key referencing Order Entity): The customer who pays.
Payment_date: The date of payment.
Payment_method: The type of payment.
Amount: The amount that has been paid.

Shipment Entity:
Shipment is the final task to do:

Shipment_id (Primary Key): A unique identifier for each shipment relationship.
Customer_id (Foreign Key referencing Customer Entity): The shipment of that customer.
Shipment_date: Date of the shipment.
City: City of that customer.
State: State of that customer.
Country: Country of the customer.
Zip_code: ZIP of that city

Cart Entity:
Customers have added items to their cart for future purchases:

Cart_id(Primary Key): A unique identifier for each cart.
Customer_id (Foreign Key referencing Customer Entity): The cart of the customer.
Product_id (Foreign Key referencing Product Entity):  The items that are added are linked to the product.
Quantity: Number of items in the cart.


Relationships are:

Each Customer can have one or more Carts (one-to-many relationship).
Each Customer can place one or more Orders (one-to-many relationship).
Each Order can have one or more payments (one-to-many relationship).
Each Order can have one shipment (one-to-one relationship).
Each product can be included in one or more Carts (many-to-many relationship).
Each Product can be part of one or more Orders (many-to-many relationship).

ER Diagram: 

Let's construct an ER diagram that vividly portrays the relationships and attributes of the entities within the Amazon schema. This ER diagram will serve as a visual representation, shedding light on the pivotal components of Amazon's data model. By employing this diagram, you'll gain a clearer grasp of the intricate interactions and connections that define the platform's dynamics.



Conclusion 

In this case study, the schema diagram for the Amazon shopping app includes several key entities, such as Customer, Product, Order, Payment, Cart, and Shipment, each with its own set of attributes and relationships. These entities work together to model the core functionality of the application, allowing customers to shop for products, place orders, make payments, manage their shopping carts, and track shipments. The diagram provides a simplified representation of the database structure, and in practice, a real-world database for a platform as comprehensive as Amazon would be more intricate, incorporating additional tables and attributes to support its extensive features and services.


