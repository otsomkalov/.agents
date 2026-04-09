---
applyTo: '**/*.fs'
---

# General

- Use latest available syntax of F# language
- Use piping instead of call chaining
- Use shortened lambdas instead of full declaration (`_.Method()` over `fun x -> x.Method()`)
- Appending new code to the end of the file
- Use `Task.FromResult()` instead of `task { return ... }`
- Omit parentheses for single-argument functions
- Avoid using anonymous records; prefer named `type` records instead
- Prefer full names for the variables
- Prefer `match` to `if-then-else`
- Prefer `Async` methods to their sync alternatives
- Use extensions functions for `Task` from `FsToolkit.ErrorHandling`

# Tests

- Use class `type` instead of module for unit tests
- Do not add `Tests` suffix to types with unit tests
- Use `NSubstitute` library to mock interfaces
- Declare and initialize mocks as `type` fields
- Use assertion checks from `FsUnit` and `FsUnit.xUnit` libraries
- Setup mocks before entering `task` computational expression
- Do not add `Mock` suffix to mock variable names
- Do not call `|> ignore` in case if mock is set up inside type `member`
- 
