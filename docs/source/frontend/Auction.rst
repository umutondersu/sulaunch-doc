Auction Component
==========================

The ``Auction`` component is found at:

.. code-block:: bash

   frontend_react/src/components/Auction.js

Overview
--------
The ``Auction`` component is a fundamental component of a frontend React application for handling auctions, particularly in the context of a Decentralized Application (DApp) or blockchain-related project. It is found in the ``frontend_react/src/components/`` directory and is named ``Auction.js``. It makes use of the ``ethers.js`` library for interaction with the Ethereum blockchain and employs the InterPlanetary File System (IPFS) for decentralized file storage.

Key Features
------------

- Manages states related to auction details, images, finish time, current data, loading status, and historic data.
- Uses React's ``useState`` and ``useEffect`` hooks for state management and side-effects handling.
- Interacts with the ``UpgradeableAuctions`` smart contract on the Ethereum blockchain.
- Utilizes multiple functions to fetch and manipulate auction data, including historical data.
- Contains a variety of auction types with corresponding information and controls.
- Renders progress circular progress bars to display the progress of the auction and sold token progress.
- Includes the ``PriceChart`` component to visually represent price data over time.
- Handles downloading of files from IPFS.
- Uses the Mantine UI library for theming and notifications.
