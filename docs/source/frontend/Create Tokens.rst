The CreateTokens Component
==========================

The ``CreateTokens`` component is found at:

.. code-block:: bash

   frontend_react/src/components/CreateTokens.js

Overview
--------

``CreateTokens`` is a React component responsible for creating tokens in the application. It leverages the ``ethers.js`` library to interact with Ethereum-based contracts. User can input the name, symbol, and total supply of the token to be created. 

Key Features
------------

- **State Management:** It uses React's useState hook to manage state within the component.

- **Ethereum Interactions:** Interacts with Ethereum contracts through the ``ethers.js`` library.

- **Error Handling:** Error messages are displayed to the user via the Mantine NotificationsProvider.

- **Input Handling:** Handles user input for token parameters such as tokenName, tokenSymbol, and totalSupply.

- **Contract Interaction:** The component leverages the Maestro contract's createToken function to mint new tokens.

- **Toast Notifications:** Handles display of toast notifications via Mantine's NotificationsProvider.

