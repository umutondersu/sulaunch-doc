Event Debug Controller
======================

The ``EventDebugController`` is used for debugging purposes and to check the whitelisting status of a user. It is located at:

.. code-block:: none

    backend_dotnet\Controllers\EventDebugController.cs

Routes
------

**Debug:**

.. http:get:: /EventDebug/Debug

   Retrieves the project evaluation event logs.

   :resjson obj response: The service response object.

**Debug Remove:**

.. http:get:: /EventDebug/DebugRemove/{address}

   Retrieves the whitelist removal event logs for a given wallet address.

   :param string address: The wallet address of the user.
   :resjson obj response: The service response object.

**Debug Add:**

.. http:get:: /EventDebug/DebugAdd/{address}

   Retrieves the whitelist insertion event logs for a given wallet address.

   :param string address: The wallet address of the user.
   :resjson obj response: The service response object.

**Is WhiteListed:**

.. http:get:: /EventDebug/Whitelisted/{address}

   Checks if the user with the given wallet address is whitelisted.

   :param string address: The wallet address of the user.
   :resjson bool response: A boolean indicating whether the user is whitelisted or not.