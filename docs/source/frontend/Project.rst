Project Component
==========================

The `Project` component is found at:

.. code-block:: bash

    frontend_react/src/components/Project.js

Overview
--------

The `Project` component is a key part of a frontend React application likely designed for a Decentralized Application (DApp) or blockchain-related project. It employs the `ethers.js` library for interaction with the Ethereum blockchain and uses the InterPlanetary File System (IPFS) for decentralized file storage.

Key Features
--------

- Manages a multitude of states for project information, markdown description, whitelisting status, and more.
- Uses React's ``useState`` and ``useEffect`` hooks for state management and updating.
- Interacts with the ``ProjectRegister`` smart contract on the Ethereum blockchain.
- Handles user navigation between routes.
- Includes functions for editing and submitting changes, as well as fetching files from IPFS.
- Utilizes cookies for likely user authentication purposes.
