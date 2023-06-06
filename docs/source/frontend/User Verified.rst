=========================
UserVerified Component
=========================

The ``UserVerified`` component is found at:

.. code-block:: bash

   frontend_react/src/components/UserVerified.js


Overview
=========
The ``UserVerified.js`` file defines a single React functional component named ``UserVerified``. This component is displayed to the user when their email address has been successfully verified.

Description
============
The ``UserVerified`` component is a simple component that displays a message to the user confirming their email verification and welcoming them to enjoy using SuLaunch. After a delay of three seconds, the user is automatically redirected to the home page.

Features
=========
1. **Redirection**: Uses the 'react-router-dom' library's ``useNavigate`` hook to perform the redirection after a delay.

2. **Delay Mechanism**: Uses a custom delay function wrapped in a Promise to create a delay before performing the redirection.

3. **useEffect Hook**: Uses React's useEffect hook to call the delay function and navigate function when the component is first rendered.

4. **Styling and Layout**: Uses inline CSS styling to center the message text vertically and horizontally in the viewport. Also sets the font family, font weight, and font size of the message.

Usage
=====
The UserVerified component is used when a user's email address has been successfully verified. It informs the user of the successful verification and redirects them to the home page after a short delay.
