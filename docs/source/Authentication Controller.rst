Authentication Controller
=========================

The ``AuthenticationController`` handles user authentication and registration. It is located at:

.. code-block:: none

    backend_dotnet\Controllers\AuthenticationController.cs

Routes
------

**Login:**

.. http:post:: /Authentication/Login

   Authenticates the user with their credentials.

   :reqjson obj request: The user login request object.
   :resjson obj response: The service response object.

**Register:**

.. http:post:: /Authentication/Register

   Registers a new user with the provided information.

   :reqjson obj request: The user registration request object.
   :resjson obj response: The service response object.

**Verify Email:**

.. http:get:: /Authentication/verify-email

   Verifies the user's email address with a provided token.

   :query string email: The user's email address.
   :query string token: The email verification token.
   :resjson obj response: The service response object.

**Get Nonce:**

.. http:get:: /Authentication/GetNonce/{address}

   Retrieves the nonce for a given wallet address.

   :param string address: The wallet address of the user.
   :resjson obj response: The service response object.
