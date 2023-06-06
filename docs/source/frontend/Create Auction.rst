.. _CreateAuction-component:

CreateAuction Component
=========================

Location
-----------

The ``CreateAuction`` component is located at:

.. code-block:: bash

   frontend_react/src/components/CreateAuction.js

Overview
-----------

The ``CreateAuction`` component handles the creation of a new auction on the blockchain. It offers a selection of different auction types for users and generates the appropriate form for the selected auction type where users can specify the necessary parameters.

Key Features
-----------------

1. **Auction Type Selection:** The component provides several options for the auction type, such as uncapped auction, pseudo capped auction, order book FCFS auction, FCFS auction, Dutch auction, orderbook Dutch auction, and strict Dutch auction.

2. **Dynamic Form Generation:** Based on the selected auction type, the component dynamically generates the necessary input fields for the user.

3. **Auction Creation:** This component interacts with the blockchain via the Maestro contract to create an auction with the specified parameters. 

4. **Database Update:** After successful creation of the auction on the blockchain, it updates the database to reflect the created auction.

5. **Error Handling and Notifications:** The component provides feedback to the user via notifications, including success notifications and error messages.

