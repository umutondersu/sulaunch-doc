Dutch Auction Bid Event
=======================


**Class**: `DutchAuctionBidEventDTO`

Properties:

1. `sender`
   - **Type**: `string`
   - **Description**: Represents the address of the bidder who submitted the bid.

2. `Amount`
   - **Type**: `uint256`
   - **Description**: Represents the amount of the bid.

3. `Price`
   - **Type**: `uint256`
   - **Description**: Represents the price of the bid.

This class is decorated with the `[Event("BidSubmission")]` attribute, indicating that it represents an event with the name "BidSubmission". It implements the `IEventDTO` interface provided by the `Nethereum.Contracts` namespace.

Please note that any required imports or namespace declarations should be included in your actual code, which have been omitted here for brevity.
