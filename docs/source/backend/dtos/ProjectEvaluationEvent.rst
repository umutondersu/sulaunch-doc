Project Evaluation Event
========================


Class: ProjectEvaluationEventDTO

* Attributes:
    * `[Event("ProjectEvaluation")]`: Decorates the class to indicate its association with the "ProjectEvaluation" event.
* Implements: `IEventDTO`

Properties:

1. `Hash`
    * Type: `byte[]`
    * Attribute: `[Parameter("bytes32", "projectHash", 1, true)]`
        * Represents an indexed parameter of type "bytes32" with a name of "projectHash" and an order of 1.
    * Description: Represents the project hash as a byte array.

2. `isApproved`
    * Type: `bool`
    * Attribute: `[Parameter("bool", "isApproved", 2, false)]`
        * Represents a non*indexed parameter of type "bool" with a name of "isApproved" and an order of 2.
    * Description: Represents whether the project is approved.

This class is designed to deserialize the event data for the "ProjectEvaluation" event when working with Ethereum smart contracts in the backend of your project.

Please note that you might need to import additional dependencies and namespaces in your actual code, which have been excluded here for brevity.
