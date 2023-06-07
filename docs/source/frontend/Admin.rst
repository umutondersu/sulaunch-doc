=======================
Admin Component
=======================

The ``Admin`` component is found at:

.. code-block:: bash

   frontend_react/src/components/Admin.jsx

Overview
=========
The ``Admin.jsx`` file defines a single React functional component named ``Admin``. This component provides administrative control over users, projects, and auctions in the system.

Description
============
The ``Admin`` component displays a tab-based interface with three sections: "User Operations", "Project Operations", and "Auction Operations". Each section is filled with different subcomponents, namely UserBox, ProjectBox, and AuctionBox respectively. The role of each subcomponent is to manage the corresponding section. 

Features
=========
1. **Tab Interface**: Utilizes the Tabs, TabList, TabPanels, Tab, and TabPanel components from the '@chakra-ui/react' library to create a tab-based interface.

2. **Section Management**: Each section/tab has its associated Box component (UserBox, ProjectBox, AuctionBox) for managing operations related to users, projects, and auctions.

3. **State Management**: Uses the React ``useState`` hook for managing the selected user in the UserBox component.

4. **Notification**: Integrates the ``useToast`` function from the '@chakra-ui/react' library for displaying notifications to the admin.

Usage
=====
The Admin component is intended for use by system administrators for management of users, projects, and auctions within the system.
