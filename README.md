# Warehouse-Management-System

LIVE: https://www.warehousesystem.ovh/

TEST USER: test@test.com <br />
TEST PASSWORD: Test123%

To fully use the application you need to allow your camera due to the scanning functionality.

## Technologies used:
 #### Fronted: react, typescript, scss, zustand, react-query, framermotion and other libraries
 
 #### Backend: express, typescript, prisma, mysql
 
 #### Deploy: docker, linux, vps

## How does the application work?

 ### Adding product model
  First, we must create a product model in the cms in order to see products in the shop
  <br><br>
  ![Add product model](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/add-prod.png?raw=true)
   <br><br>
  As soon as we have added one, we will be able to see the product in the store
  <br><br>
![Shop view](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/Zrzut%20ekranu%202023-09-1%20o%2019.29.42.png?raw=true)
### Creating a location and assigning a pallet
 To refill a product stock we need to create a location and a pallet where products will be stored.
 In CMS -> MANAGMENT -> CREATE we have an option to create a location and a pallet.
 <br><br>
 ![Create view](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/create-view.png?raw=true)
 <br><br>
 Once we click "location", a location is created
 <br><br>
 ![Location creation](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/create-location.png?raw=true)
 <br><br>
 Now we should print the saved location QR code and put it into the rack/place where the location should be.
 By default, the location doesn't contain any pallet, so we need to create one.
 To create a pallet we need to scan a location QR code, or we can type it in manually in case of a broken location label.
 <br><br>
 ![Pallet creation](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/create-pallet.png?raw=true)
 <br><br>
 After the pallet has been created we can see it is attached to the location that we provided.
 <br><br>
 ![Pallet inspection](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/pallet-inspection.png?raw=true)
 <br><br>
 ### Product refill
 Finally after creating location and pallet we are ready to refill product quantity.
 However, before we proceed, we should print the pallet label and attach it to the pallet itself.
 To refill product we should go to MANAGMENT -> REFILL and scan product that we want to put on a pallet.
 <br><br>
 ![Product refill](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/scan-product.png?raw=true)
 <br><br>
 Next we need to scan the pallet label on which products should be placed
 <br><br>
 ![Scan pallet](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/scan-pallet.png?raw=true)
 <br><br>
 And the last step, provide the quantity (how many items of this product type you want to put on the pallet)
 <br><br>
 ![Provide quantity](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/provide-quantity.png?raw=true)
 <br><br>
 Upon successfully adding products to the pallet, we will be able to see that the stock has been updated
 <br><br>
  ![Stock view](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/stock-view.png?raw=true)
  ![Inspect full location](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/inspect-full-location.png?raw=true)
  <br><br>
 ### Creating an order
  <br><br>
  Now we are able to add items to the cart and place an order.
  <br><br>
  ![Add to the cart](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/add-cart.png?raw=true)
  ![The cart](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/cart.png?raw=true)
  ![Order creation](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/order-creation.png?raw=true)
  ![Payment](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/payment.png?raw=true)
  ![Payment Success](https://github.com/Hero1230/Warehouse-management-System/blob/master/images-gh/success-payment.png?raw=true)
 ### Order picking (picking an order)
  
  
## Features
### Shop prototype
  - add/remove products from the cart
  - create an order

### WMS
  - register/login
  - create product and add it to the shop
  - create location
  - create pallet
  - refill products
  - re-assign product to a different pallet
  - inspect all locations
  - inspect all products
  - inspect all orders
  - inspect location via scanning QR
  - inspect product via scanning barcode
  - order picking (pick all ordered items, and forward it to the shipment zone)
