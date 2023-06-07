User
====

**Class**: `User`

Properties:

1. `Id`
    * **Type**: `int`
    * **Description**: Represents the ID of the user.

2. `Name`
    * **Type**: `string`
    * **Description**: Represents the name of the user.

3. `Surname`
    * **Type**: `string`
    * **Description**: Represents the surname of the user.

4. `Address`
    * **Type**: `string`
    * **Description**: Represents the address of the user.

5. `MailAddress`
    * **Type**: `string?`
    * **Description**: Represents the email address of the user. It can be nullable.

6. `Username`
    * **Type**: `string`
    * **Description**: Represents the username of the user.

7. `Role`
    * **Type**: `string`
    * **Description**: Represents the role of the user. It is set to a default value from `UserRoleConstants.BASE`.

8. `Nonce`
    * **Type**: `Nullable<int>`
    * **Description**: Represents the nonce value associated with the user. It can be nullable.

9. `VerificationToken`
    * **Type**: `string`
    * **Description**: Represents the verification token for the user.

10. `VerificationExpiration`
     * **Type**: `DateTime?`
     * **Description**: Represents the expiration date and time for the verification token. It can be nullable.

11. `IsVerified`
     * **Type**: `bool`
     * **Description**: Represents whether the user is verified or not.

Please note that any required imports or namespace declarations should be included in your actual code, which have been omitted here for brevity.
