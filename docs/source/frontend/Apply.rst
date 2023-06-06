=======================
Apply Component
=======================
The ``Apply`` component is found at:

.. code-block:: bash

    rontend_react/src/components/Apply.js

Overview
------------


``Apply`` is a React component that provides the user interface for a form that accepts project details and saves them in a blockchain database.

Key Features
------------

* **User Authentication**: Uses axios to handle API requests for user authentication, and uses cookies for managing tokens.
* **Project Registration**: Users can submit project details including the project name, a description, a whitepaper (in PDF format), and an image. This data is sent to a backend server and also added to the blockchain.
* **Notification System**: Uses the Mantine Notification system to show progress and result notifications.
* **File Uploads**: Supports uploading of PDF and image files. The PDF is meant to be the project whitepaper and the image is the project image. Both are processed and stored as hexadecimal strings.
* **Form Validation**: The form uses React Bootstrap's built-in validation.
* **File Download**: There is a function that converts the whitepaper file from a hexadecimal string back to a file and triggers a download.
* **Ethereum Smart Contract Interaction**: The component interacts with an Ethereum smart contract to register the project.
* **React Context**: Uses the UserContext for managing user data.

Functions
---------

The following list includes some of the functions that the Apply component uses:

* ``connectToContract``: This function is used to connect with an Ethereum smart contract and register a project.
* ``handleDB``: This function posts the project details to the backend server and saves them in a database.
* ``downloadFile``: This function triggers the download of the whitepaper file.
* ``handleInput``: This function handles the form inputs.
* ``handleSubmit``: This function handles form submission.
* ``SetWhitePaper``: This function handles the uploading and processing of the whitepaper file.
* ``SetImage``: This function handles the uploading and processing of the image file.

Sub-Components
--------------

* **MyDropzone**: This is a dropzone component for uploading files. It handles the drag-and-drop file uploading process.

Related Components
------------------

* ``UserContext``: React context for managing user data.
* ``NotificationsProvider``: Mantine component used for managing notifications.

