User Controller
===============

The ``UserController`` manages user-related actions such as retrieving, updating, and deleting user information, managing project permissions, and handling project invitations. It is located at:

.. code-block:: none

    backend_dotnet\Controllers\UserController.cs

Routes
------

- ``GET /user/get``: Retrieves the user information.
- ``PUT /user/update``: Updates the user information.
- ``DELETE /user/delete``: Deletes the user's own account.
- ``DELETE /user/deleteuser/{id:int}``: Deletes a user account as an admin.
- ``POST /user/invite``: Invites a user to a project.
- ``PUT /user/invitationreply``: Allows the user to reply to a project invitation.
- ``GET /user/getall``: Retrieves all users (admin only).
- ``GET /user/learnusercount``: Retrieves the total user count.
- ``GET /user/getcoowners/{projectID:int}``: Retrieves co-owners of a project.
- ``DELETE /user/removecollab``: Removes a collaborator from a project.
- ``PATCH /user/updaterole/{address}/{role}``: Updates the role of a user (admin only).