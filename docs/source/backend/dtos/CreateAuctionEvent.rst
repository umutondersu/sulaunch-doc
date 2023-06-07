Create Auction Event
====================

**Class**: `CreateAuctionEventDTO`

Properties:

1. `Creator`
    * **Type**: `string`
    * **Description**: Represents the address of the creator who initiated the auction.

2. `Auction`
    * **Type**: `string`
    * **Description**: Represents the address of the created auction.

3. `AuctionType`
    * **Type**: `string`
    * **Description**: Represents the type of the auction.

4. `FileHash`
    * **Type**: `byte[]`
    * **Description**: Represents the hash of the associated file.

This class is decorated with the `[Event("CreateAuctionEvent")]` attribute, indicating that it represents an event with the name "CreateAuctionEvent". It implements the `IEventDTO` interface provided by the `Nethereum.Contracts` namespace.

Please note that any required imports or namespace declarations should be included in your actual code, which have been omitted here for brevity.



