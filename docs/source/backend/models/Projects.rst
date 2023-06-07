Projects
========

**Class**: `Project`

Properties:

1. `ProjectID`
    * **Type**: `int`
    * **Description**: Represents the ID of the project.

2. `ProjectName`
    * **Type**: `string`
    * **Description**: Represents the name of the project.
    * **Required**: Yes

3. `Date`
    * **Type**: `Nullable<System.DateTime>`
    * **Description**: Represents the date of the project.

4. `ViewerAccepted`
    * **Type**: `bool`
    * **Description**: Indicates whether the viewer has accepted the project.

5. `IsAuctionCreated`
    * **Type**: `bool`
    * **Description**: Indicates whether an auction has been created for the project.

6. `IsAuctionStarted`
    * **Type**: `bool`
    * **Description**: Indicates whether the auction for the project has started.

7. `FileHash`
    * **Type**: `string`
    * **Description**: Represents the hash of the project file.

8. `ProjectDescription`
    * **Type**: `string`
    * **Description**: Represents the description of the project.
    * **Required**: Yes

9. `Rating`
    * **Type**: `double`
    * **Description**: Represents the rating of the project.

10. `Status`
    * **Type**: `string`
     * **Description**: Represents the status of the project.
     * **Default**: `ProjectStatusConstants.PENDING`

11. `MarkDown`
    * **Type**: `string`
    * **Description**: Represents the Markdown content of the project.

12. `ProposerAddress`
    * **Type**: `string`
    * **Description**: Represents the address of the project proposer.

13. `ViewerAcceptedAddress`
    * **Type**: `string`
    * **Description**: Represents the address of the viewer who accepted the project.

Please note that any required imports or namespace declarations should be included in your actual code, which have been omitted here for brevity.
