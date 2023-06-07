Project
=======


**Class**: `ProjectDTO`

Properties:

1. `ProjectID`
    * **Type**: `int`
    * **Description**: Represents the unique identifier of the project.

2. `ProjectName`
    * **Type**: `string`
    * **Default Value**: `""` (empty string)
    * **Description**: Represents the name of the project.

3. `Date`
    * **Type**: `Nullable<System.DateTime>`
    * **Description**: Represents the date associated with the project.

4. `IsAuctionCreated`
    * **Type**: `bool`
    * **Default Value**: `false`
    * **Description**: Represents whether an auction is created for the project.

5. `ProjectDescription`
    * **Type**: `string?` (nullable string)
    * **Description**: Represents the description of the project.

6. `ImageUrl`
    * **Type**: `string?` (nullable string)
    * **Default Value**: `null`
    * **Description**: Represents the URL of the project's image.

7. `Rating`
    * **Type**: `double`
    * **Default Value**: `0`
    * **Description**: Represents the rating of the project.

8. `Status`
    * **Type**: `string`
    * **Default Value**: `ProjectStatusConstants.PENDING`
    * **Description**: Represents the status of the project. The default value is obtained from the `ProjectStatusConstants` class in the `SU_COIN_BACK_END.Constants` namespace.

9. `MarkDown`
    * **Type**: `string`
    * **Default Value**: `""` (empty string)
    * **Description**: Represents the markdown content associated with the project.

10. `FileHash`
    * **Type**: `string`
    * **Default Value**: `""` (empty string)
    * **Description**: Represents the hash of a file associated with the project.

11. `ProposerAddress`
    * **Type**: `string?` (nullable string)
    * **Default Value**: `null`
    * **Description**: Represents the address of the project proposer.

12. `ViewerAcceptedAddress`
    * **Type**: `string?` (nullable string)
    * **Default Value**: `null`
    * **Description**: Respresents the address of the user that accept.
