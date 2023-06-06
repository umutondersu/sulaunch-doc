Profile Page Component
==========================

The ``Profile Page`` component is found at:

.. code-block:: bash

   frontend_react/src/components/ProfilePage.js

Overview
--------

ProfilePage.js is a React component that provides the profile page of a user. The page displays user information and their associated projects. The file is primarily composed of functional components, hooks, and several asynchronous operations to interact with the back-end service.

Features
--------

- **User Information:** Displays user's name, surname, email, and username. There is an option for users to edit their information.

- **Projects:** Shows all the projects the user has permission to access. Each project card has options to edit, delete, and send an invitation request for the project.

- **Invitations:** Displays all the invitations the user has received. Each invitation card has options to accept or reject the invitation.

- **Loading State:** Includes a loading state to handle asynchronous operations.

