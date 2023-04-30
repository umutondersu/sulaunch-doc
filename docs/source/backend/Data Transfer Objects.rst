Data Transfer Objects
======================

``Data Transfer Object`` (shortened as ``DTO``), is a design pattern used in software development to transfer data between layers of an application. In .NET, DTOs are typically used to transfer data between the business logic layer and the presentation layer or between different components of a distributed application.

In this project, ``DTO`` classes are primarily used to model the data coming from and going to the Solidity Smart Contract. They contain classes representing Smart Contract events and function outputs. The Nethereum library is used to interact Smart Contracts in the .NET environment. Nethereum provides attributes like Event, Parameter, and FunctionOutput to define and map these classes to their respective smart contract events and function outputs.



