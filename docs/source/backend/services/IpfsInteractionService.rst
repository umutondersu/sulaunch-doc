IPFS Interaction Service
========================

**Class**: `IpfsInteractionService`

Dependencies:
- `IIpfsInteractionService`: An interface for IPFS interaction.
- `Newtonsoft.Json`: A library for JSON serialization and deserialization.
- `ServiceResponse`: A generic class for encapsulating service responses.
- `MessageConstants`: A class containing message constants.

Methods:

1. `UploadToIpfs(string hexString, string? imageHex)`
    * **Parameters**:
        * `hexString`: The hexadecimal string representing the file to upload.
        * `imageHex`: The optional hexadecimal string representing an image file to upload.
    * **Return Type**: `Task<ServiceResponse<string>>`
    * **Description**: Uploads a file or a file with an image to the IPFS network. It returns the hash of the uploaded content.

2. `RemoveFromIpfs(string encodedHash)`
    * **Parameters**:
        * `encodedHash`: The encoded hash of the content to remove from IPFS.
    * **Return Type**: `Task<ServiceResponse<bool>>`
    * **Description**: Removes content from the IPFS network based on the encoded hash. It returns a boolean indicating the success of the removal operation.

Please note that the documentation provided here is a general outline. You may need to add more detailed explanations for each method based on your specific requirements.
