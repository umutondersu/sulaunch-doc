Project Register Event
======================


Class: ProjectRegisterEventDTO

* Attributes:
    * `[Event("Register")]`: Decorates the class to indicate its association with the "Register" event.
* Implements: `IEventDTO`

Properties:

1. `From`
    * Type: `string`
    * Attribute: `[Parameter("address", "from", 1, true)]`
        * Represents an indexed parameter of type "address" with a name of "from".
    * Description: Represents the address of the event sender.

2. `Hash`
    * Type: `byte[]`
    * Attribute: `[Parameter("bytes32", "projectHash", 2, false)]`
        * Represents a non*indexed parameter of type "bytes32" with a name of "projectHash".
    * Description: Represents the project hash as a byte array.

This class is utilized for deserializing event data related to the "Register" event when interacting with Ethereum smart contracts in the backend of your project.

Please ensure that you include the necessary import statements and namespaces in your actual code, which have been omitted here for conciseness.
