Controllers Introduction
========================

.. _controllers:

Controllers in this project are responsible for handling incoming HTTP requests, managing the flow of data between the client and the business logic, and sending appropriate HTTP responses based on the outcomes of the operations performed. They act as intermediaries between the front-end and the back-end services. Below is a brief introduction to each controller.

AuthenticationController
------------------------

This controller is responsible for handling user authentication, including logging in and registering new users. It also manages email verification and provides the functionality to get a nonce (a unique value) for a user's address.

EventDebugController
--------------------

The EventDebugController is designed to help debug events emitted by the blockchain contracts. It retrieves and displays event logs related to project evaluation, whitelist addition, and whitelist removal. It also checks if a user is whitelisted.

UserController
--------------

The UserController is responsible for managing user-related operations. These include retrieving user details, updating user information, deleting a user, inviting a user to a project, managing project invitations, and listing all users. This controller also handles operations related to project co-owners, removing collaboration permissions from users, and updating user roles.

ProjectController
-----------------

The ProjectController is responsible for managing project-related operations. These include creating a new project, retrieving project details, updating project information, deleting a project, listing all projects, and listing all projects a user is a member of. This controller also handles operations related to project co-owners, removing collaboration permissions from users, and updating user roles.
