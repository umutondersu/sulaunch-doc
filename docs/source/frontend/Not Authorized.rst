NotAuthorized Component
========================

The ``NotAuthorized`` component is found at:

.. code-block:: bash

   frontend_react/src/components/NotAuthorized.js

Overview
--------

The ``NotAuthorized`` component is used to display an authorization error message to the user, indicating that they do not have the necessary permissions to view the page they attempted to access. After a delay of 3000 milliseconds (3 seconds), the component automatically redirects the user to the root ('/') route.

Features
--------

1. **Redirect Delay**: Utilizes a custom ``delay`` function which returns a Promise that resolves after a specified time period. In this case, a delay of 3000 milliseconds is implemented.

2. **Navigation**: Uses the ``useNavigate`` hook from React Router DOM for navigation. After the delay, the user is redirected to the home route ('/').

3. **Styling**: The component returns a div with a centered message. The styling is applied inline and includes flexbox centering, a full viewport height, and specific font properties.

4. **Effect**: The side effect of redirecting the user after a delay is handled in the ``useEffect`` hook, which executes upon component mount.

Usage
--------

This component is intended to be used when a user tries to access a restricted page without the necessary permissions.
