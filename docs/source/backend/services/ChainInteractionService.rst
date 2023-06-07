Chain Interaction Service
=========================

**Class**: `ChainInteractionService`

Dependencies:
* `IMapper`: An object mapper for mapping between objects.
* `DataContext`: The data context for accessing the database.
* `IHttpContextAccessor`: An accessor for accessing the HTTP context.
* `Web3`: A library for interacting with Ethereum networks.

Constructor:
* Initializes the class and sets the required dependencies.
* Sets the connection timeout for the blockchain client.
* Initializes the `Web3` object with the Infura URL.

Private Methods:

1. `GetUserId()`
    * **Return Type**: `int`
    * **Description**: Retrieves the user ID from the HTTP context.

2. `GetUserAddress()`
    * **Return Type**: `string`
    * **Description**: Retrieves the user address from the HTTP context.

Methods:

1. `GetRegisterEventLogs()`:
    * **Return Type**: `Task<ServiceResponse<List<EventLog<ProjectRegisterEventDTO>>>>`
    * **Description**: Retrieves the event logs for project registration from the blockchain.

2. `GetWhiteListInsertEventLogs(string address)`:
    * **Parameters**:
        * `address`: The address for filtering the event logs.
    * **Return Type**: `Task<ServiceResponse<List<EventLog<WhitelistInsertEventDTO>>>>`
    * **Description**: Retrieves the event logs for whitelist insertions from the blockchain.

3. `GetWhiteListRemoveEventLogs(string address)`:
    * **Parameters**:
        * `address`: The address for filtering the event logs.
    * **Return Type**: `Task<ServiceResponse<List<EventLog<WhitelistRemoveEventDTO>>>>`
    * **Description**: Retrieves the event logs for whitelist removals from the blockchain.

4. `GetChainRole(string address)`:
    * **Parameters**:
        * `address`: The address of the user.
    * **Return Type**: `Task<ServiceResponse<string>>`
    * **Description**: Retrieves the chain role of a user based on their address.

5. `GetAuctionFromHash(string projectHash)`:
    * **Parameters**:
        * `projectHash`: The hash of the project.
    * **Return Type**: `Task<ServiceResponse<string>>`
    * **Description**: Retrieves the auction address associated with a project hash.

6. `IsAuctionCreatedInChain(string projectHash)`:
    * **Parameters**:
        * `projectHash`: The hash of the project.
    * **Return Type**: `Task<ServiceResponse<bool>>`
    * **Description**: Checks if an auction is created in the blockchain for a given project hash.

7. `IsAuctionStartedInChain(string projectHash)`
    * **Parameters**:
        * `projectHash`: The hash of the project.
    * **Return Type**: `Task<ServiceResponse<bool>>`
    * **Description**: Checks if an auction is started in the blockchain for a given project hash.

8. `GetProjectEvaluationEventLogs()`:
    * **Return Type**: `Task<ServiceResponse<List<EventLog<ProjectEvaluationEventDTO>>>>`
    * **Description**: Retrieves the event logs for project evaluations from the blockchain.
