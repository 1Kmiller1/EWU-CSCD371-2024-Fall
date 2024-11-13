# Assignment

## Overview

For this assignment, we are going to continue with C# object-oriented concept by expanding Assignment2 to use records, value types, enums, and developing well-formed types in general.

## Reading

Read **Chapters 9 - Introducing Structs and Records & Chapter 10 - Well Formed Typed**

## Tasks

- Define a full name record (first, last, middle) handling optional and null appropriately. ❌✔
  - Provide a comment on the full name record on why you selected to define a value or a reference type and ❌✔
  - Provide a comment on the full name record on why or why not the type is immutable. ❌✔
- Define an `IEntity` interface: ❌✔
  - Add an Id property of type `Guid` that is an init-only setter. ❌✔
  - Add a Name property that is `string`. ❌✔
- Define an abstract base class that implements `IEntity` - appropriately choosing to implement the interface explicitly or implicitly. ❌✔
  - Do not implement the `Name` property in this abstract class. ❌✔
  - Do force any derived classes to provide an implementation for `Name`. ❌✔
- Define book, student, and employee records - all with entity capabilities. ❌✔
  - Choose a thoughtful approach for the value of `Name` for each type of entity. In all cases, there should be no backing field for Name (not even one generated by an automatically implemented property) - consider a calculated property. ❌✔
  - Provide a comment on each interface **member** in each entity explaining why you implemented it implicitly or explicitly. ❌✔
  - You should consider the relationship between Student and Employee and refactor the common code shared between them. ❌✔
  - Given the properties on the full name record, you should consider which entities it makes sense to use it. ❌✔
  - Test that the equality behavior on these entities behaves as expected. ❌✔
  - Provide a comment on each interface method explaining why you implemented it implicitly or explicitly.
- Unit test the Storage class using various entities to ensure that there are no bugs.
- Code review (using TODO: comments if there are any issues - which there may not be) all logger-related classes.)
  - Pay special attention to the CreateLogger methods throughout.

## Fundamentals

- Be sure you enable:
  - Enable Nullability for all projects  ❌✔
  - Set `LangVersion` and the `TargetFramework` to the latest released versions available (preview versions optional) ❌✔
  - Ensure that you turn on code analysis for all projects(`EnableNETAnalyzers`) ❌✔
  - Ensure that you turn on `EnforceCodeStyleInBuild` ❌✔
  - Ensure that you turn on Nullability (`Nullable`) ❌✔
- **Ensure there are no errors or warnings (including code analysis warnings)** ❌✔
- **All of the above should be unit tested** ❌✔
- **Choose simplicity over complexity** ❌✔

## Extra Credit

- Refactor your project files to put common properties and/or items into a single file. ❌✔
- Convert `ILogger.CreateLogger` to a generic method. ❌✔
  - Returns the logger classes type that is to be created. ❌✔
  - Has a type parameter for the configuration type ❌✔


## Relevant APIs to know about

[System.IO.Path](https://docs.microsoft.com/dotnet/api/system.io.path) IF you find yourself using string operations to build up a file path, stop and look through the members of this static class.

[System.IO.File](https://docs.microsoft.com/dotnet/api/system.io.file) A simple class that can handle simple file reads and writes.

## See [Docs](https://github.com/IntelliTect-Samples/EWU-CSCD371-2024-Fall/blob/main/Docs/README.md)
