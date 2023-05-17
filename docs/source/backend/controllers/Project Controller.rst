Project Controller
==================

The ``ProjectController`` manages the projects and their associated actions. It is located at:

.. code-block:: none

    backend_dotnet\Controllers\ProjectController.cs

Routes
------

**Get all projects:**

.. http:get:: /Project/Get/All

   Retrieves all projects.

   :query bool withHex: Optional query parameter to include hexadecimal values.
   :resjson obj response: The service response object containing a list of projects.

**Get project by ID:**

.. http:get:: /Project/Get/{id:int}

   Retrieves a project by its ID.

   :param int id: The project ID.
   :resjson obj response: The service response object containing the project details.

**Update project:**

.. http:put:: /Project/Update

   Updates an existing project.

   :reqjson obj project: The project data to be updated.
   :resjson obj response: The service response object.

**Delete project:**

.. http:delete:: /Project/Delete/{id}

   Deletes a project by its ID.

   :param int id: The project ID.
   :resjson obj response: The service response object.

**Add project:**

.. http:post:: /Project/Add

   Adds a new project.

   :reqjson obj project: The project data to be added.
   :resjson obj response: The service response object.

**Rate project:**

.. http:put:: /Project/Rate/{id:int}/{rating}

   Rates a project.

   :param int id: The project ID.
   :param double rating: The rating value.
   :resjson obj response: The service response object.

**Get projects by status:**

.. http:get:: /Project/GetByStatus/{status}

   Retrieves projects by their status.

   :param string status: The project status.
   :resjson obj response: The service response object containing a list of projects.

**Change project status:**

.. http:put:: /Project/ChangeStatus/{id:int}

   Changes the status of a project.

   :param int id: The project ID.
   :resjson obj response: The service response object.

**Update project markdown:**

.. http:put:: /Project/UpdateMarkDown/{id:int}/{markdown}

   Updates a project's markdown.

   :param int id: The project ID.
   :param string markdown: The updated markdown content.
   :resjson obj response: The service response object.

**Get all permissioned projects:**

.. http:get:: /Project/GetAllPermissioned/{withHex}

   Retrieves all permissioned projects.

   :query bool withHex: Optional query parameter to include hexadecimal values.
   :resjson obj response: The service response object containing a list of projects.

**Get all invitations:**

.. http:get:: /Project/GetAllInvitations

   Retrieves all project invitations.

   :resjson obj response: The service response object containing a list of invitations.

**Get top N rated projects:**

.. http:get:: /Project/GetProjects/{numberOfProjects:int}

   Retrieves the top N rated projects.

   :param int numberOfProjects: The number of projects to retrieve.
   :resjson obj response: The service response object containing a list of projects.

**Get all project file hashes:**

.. http:get:: /Project/GetAllHashes/{areOnlyAuctionsStarted}

   Retrieves all project file hashes.

   :query bool areOnlyAuctionsStarted: Optional query parameter to filter projects with auctions started.
   :resjson obj response: The service response object containing a list of project file hashes.

**Reply to project preview:**

.. http:put:: /Project/ViewerReply/{id:int}/{reply}

   Submits a reply to a project preview.

   :param int id: The project ID.
   :param bool reply: The viewer's reply (true or false).
   :resjson obj response: The service response object.
