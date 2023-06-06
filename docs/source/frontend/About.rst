===================
About Component
===================
The ``About`` component is found at:

.. code-block:: bash

   frontend_react/src/components/About/About.js

Overview
=========
The ``About.js`` file defines a single React functional component named ``About``. This component presents information about the project and the team of developers who created it.

Description
============
The ``About`` component has two main sections: an overview of the "SuLaunch" project and a list of project members. The overview section describes the project's aims, motivation, and the technologies used. The project members' section displays a list of team members, their roles, and their contact information.

Features
=========
1. **Project Information**: Provides a detailed description of the SuLaunch project, its aims, technology used, and motivation.
   
2. **Project Members**: Lists the team members who developed the project, along with their roles, contact information, and images.

3. **Data Mapping**: Uses the map function to render each developer's information from a local array of developer objects.

4. **Styling and Layout**: Uses various components from the '@mantine/core' library, such as Text, Avatar, Card, Image, Group, and Badge, to create a visually pleasing and well-structured layout.

5. **Conditional Rendering**: Utilizes a ternary operator to conditionally render either an Image or an Avatar component based on the availability of the developer's image URL.

Usage
=====
The About component is used to provide information about the SuLaunch project and the team of developers who worked on it. It can be used in any part of the application where this information needs to be displayed.
