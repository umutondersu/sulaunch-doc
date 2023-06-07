Admin Change Event
==================

**Class**: `AdminChangeEventDTO`

Properties:

1. `From`
    * **Type**: `address`
    * **Description**: Represents the address of the previous admin.

2. `To`
    * **Type**: `address`
    * **Description**: Represents the address of the new admin.

This class is decorated with the `[Event("AdminChange")]` attribute, indicating that it represents an event with the name "AdminChange". It implements the `IEventDTO` interface provided by the `Nethereum.Contracts` namespace.

Please note that any required imports or namespace declarations should be included in your actual code, which have been omitted here for brevity.
