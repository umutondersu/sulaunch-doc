=========================
Viewer Component
=========================

The ``Viewer`` component is found at:

.. code-block:: bash

   frontend_react/src/components/Viewer.js


Overview
=========
The ``Viewer.js`` file defines a single React functional component called ``Viewer``. This component is responsible for displaying a list of projects and providing functionality to manage these projects.

Description
============
The ``Viewer`` component retrieves a list of projects from a backend server, displays them in a table, and allows the user to accept, reject, or download each project's PDF file.

Features
=========
1. **State Management**: Utilizes React's ``useState`` and ``useEffect`` hooks for managing component state and side effects. The state includes a list of projects and details of each project like ID and fileHash.

2. **API Calls**: Uses the Axios library to send HTTP requests to a backend server. The server's URL is stored in a separate ``config`` file.

3. **Authentication**: Includes an authentication header in API requests. This header is set to a Bearer token stored in a cookie.

4. **File Downloading**: Downloads a project's PDF file from the IPFS (InterPlanetary File System) when the corresponding button is clicked. The downloaded file is then saved to the user's device.

5. **Project Management**: Allows the user to accept or reject a project. When a project is accepted or rejected, an API request is sent to update the project's status on the backend server.

Usage
=====
The Viewer component is intended to be used when there is a need to display a list of projects and allow a user to manage these projects by accepting, rejecting, or downloading their associated files.
