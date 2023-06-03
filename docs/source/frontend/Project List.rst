The ProjectList Component
=========================

The ``ProjectList`` component is located at:

.. code-block:: bash

   frontend_react/src/components/ProjectList.js

Overview
--------

The ``ProjectList`` component displays a list of projects in the web application. It is responsible for fetching the project data from the backend, allowing for filtering by project status, and rendering the project data in a grid format.

Key Features
------------

- **Data Fetching:** Fetches project data from the backend using ``axios``.

- **Role and Token Handling:** Retrieves the user role from the token stored in cookies. It uses this to determine what projects should be displayed based on the role of the user.

- **Project Filtering:** Allows for filtering the displayed projects by their status (e.g., all, approved, pending, rejected).

- **Grid Display:** Displays projects in a grid format using the ``SimpleGrid`` component from ``@chakra-ui/react``.

- **Loading State Handling:** Displays a loading icon while project data is being fetched, transitioning to the actual content once data is ready.
