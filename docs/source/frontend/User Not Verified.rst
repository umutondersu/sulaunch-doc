=============================
UserNotVerified Component
=============================

The ``UserNotVerified`` component is found at:

.. code-block:: bash

    frontend_react/src/components/UserNotVerified.js

Overview
=========
The ``UserNotVerified.js`` file defines a single React functional component named ``UserNotVerified``. This component is displayed to the user when the verification link they are trying to use has expired.

Description
============
The ``UserNotVerified`` component is a simple component that displays a message to the user stating that the verification link they are trying to use has expired, and instructs them to fill out the sign-up form again. After a delay of three seconds, the user is automatically redirected to the home page.

Features
=========
1. **Redirection**: Uses the 'react-router-dom' library's ``useNavigate`` hook to perform the redirection after a delay.

2. **Delay Mechanism**: Uses a custom delay function wrapped in a Promise to create a delay before performing the redirection.

3. **useEffect Hook**: Uses React's useEffect hook to call the delay function and navigate function when the component is first rendered.

4. **Styling and Layout**: Uses inline CSS styling to center the message text vertically and horizontally in the viewport. Also sets the font family, font weight, and font size of the message.

Usage
=====
The UserNotVerified component is used when the user tries to access a resource with an expired verification link. It informs the user of the situation and redirects them to the home page after a short delay.
