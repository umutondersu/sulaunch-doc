Auctions Component
=====================

Location
-----------

The ``Auctions`` component is located at:

.. code-block:: bash

   frontend_react/src/components/Auctions.js

Overview
-----------

The ``Auctions`` component retrieves and displays a list of all auctions from the blockchain. It allows filtering auctions based on their status, like "Off", "Running", "Paused", "Ended", or "All". Each auction is represented as a card, utilizing the `AuctionCard` component.

Key Features
-----------------

1. **Auction Retrieval:** This component retrieves auctions from the blockchain using the Maestro contract. 

2. **Auction Filtering:** Auctions can be filtered by their status, allowing users to view auctions that are off, running, paused, ended, or all auctions regardless of status.

3. **Auction Display:** Each auction is displayed as a card on the user interface, which includes key information about the auction such as the project name, description, and auction type.

4. **Error Handling and Notifications:** The component provides feedback to the user via notifications in the event of errors. It utilizes the `NotificationsProvider` from `@mantine/notifications` for this purpose.

5. **Loading State:** The component displays a loading icon while it fetches the auction data from the blockchain.

