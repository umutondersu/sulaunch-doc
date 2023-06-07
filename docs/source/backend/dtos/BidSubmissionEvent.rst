Bid Submission Event
====================

**Class**: `BidSubmissionEventDTO`

Properties:

1. `Sender`
   - **Type**: `address`
   - **Description**: Represents the address of the sender who submitted the bid.

2. `Amount`
   - **Type**: `uint256`
   - **Description**: Represents the amount of the bid.

This class is decorated with the `[Event("BidSubmission")]` attribute, indicating that it represents an event with the name "BidSubmission". It implements the `IEventDTO` interface provided by the `Nethereum.Contracts` namespace.

Please note that any required imports or namespace declarations should be included in your actual code, which have been omitted here for brevity.
