=========================
HowToUse Component
=========================

The ``HowToUse`` component is found at:

.. code-block:: bash

   frontend_react/src/components/HowToUse.js

Overview
=========

``HowToUse`` is a React component that is primarily used to redirect users to an external website that contains the 'how to use' guide of the project.

Key Features
------------

* **Redirect**: On component mount, the useEffect React hook is used to redirect the user to the "how to use" guide hosted on an external site (`https://umutondersu.github.io/Sulaunch/`).

* **Placeholder**: While the page is redirecting, a message "Redirecting..." is displayed to the user. This can be replaced with a loading gif or any other visual cue to indicate the ongoing redirection.

Functions
---------

The component makes use of the following JavaScript function:

* ``useEffect``: This is a React hook that is used to perform side-effects in the component. In this case, it is used to execute the redirection when the component is rendered.

Related Components
------------------

* ``BrowserRouter, Routes, Route, Link``: These are components from the `react-router-dom` package, which is used for routing in React applications. Although imported in this file, they do not appear to be used within the ``HowToUse`` component. If not needed for other parts of the file, these imports could potentially be removed.

