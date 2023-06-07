Authentication Service
======================

**Class**: `AuthenticationService`

Dependencies:
* `IMapper`: An object mapper for mapping between objects.
* `DataContext`: The data context for accessing the database.
* `IHttpContextAccessor`: An accessor for accessing the HTTP context.
* `IConfiguration`: The configuration settings.
* `IChainInteractionService`: A service for interacting with the blockchain.

Constructor:
* Initializes the class and sets the required dependencies.

Private Methods:

1. `GenerateVerificationToken()`
    * **Return Type**: `string`
    * **Description**: Generates a verification token used for email verification.

2. `SendVerificationEmail(string email, string token)`
    * **Parameters**:
        * `email`: The email address of the user.
        * `token`: The verification token.
    * **Description**: Sends a verification email to the user with the provided email address and verification token.

3. `GetNonce(string address)`
    * **Parameters**:
        * `address`: The user's Ethereum address.
    * **Return Type**: `Task<ServiceResponse<int>>`
    * **Description**: Retrieves the nonce value for the user with the provided Ethereum address.

4. `Login(UserLoginRequest request)`
    * **Parameters**:
        * `request`: The login request containing the user's Ethereum address and signed message.
    * **Return Type**: `Task<ServiceResponse<string>>`
    * **Description**: Handles the user login process, including address and signature verification.

5. `VerifyEmail(string email, string token)`
    * **Parameters**:
        * `email`: The user's email address.
        * `token`: The verification token.
    * **Return Type**: `Task<ServiceResponse<string>>`
    * **Description**: Verifies the user's email address using the provided email and verification token.

6. `Register(UserRegisterRequest request)`
    * **Parameters**:
        * `request`: The user registration request containing user details and a signed message.
    * **Return Type**: `Task<ServiceResponse<string>>`
    * **Description**: Handles the user registration process, including email verification and user creation.

7. `UserExists(string address, string email, string username)`
    * **Parameters**:
        * `address`: The user's Ethereum address.
        * `email`: The user's email address.
        * `username`: The user's username.
    * **Return Type**: `Task<bool>`
    * **Description**: Checks if a user with the provided Ethereum address, email address, or username already exists.

8. `UserNameExists(string username)`
    * **Parameters**:
        * `username`: The username to check.
    * **Return Type**: `Task<bool>`
    * **Description.
