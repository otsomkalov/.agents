---
applyTo: '**/*.fs'
---

# General

- Prefer piping to call chaining
- Prefer shortened lambdas to full declaration (`_.Method()` over `fun x -> x.Method()`)
- Prefer appending new code to the end of the file
- Use `Task.FromResult()` instead of `task { return ... }`
- Omit parentheses for single-argument functions
- Avoid using anonymous records; prefer named `type` records instead
- Prefer full names for the variables
- Prefer `match` to `if-then-else`
- Prefer `Async` method to their sync alternatives

# Tests

- Prefer class `type` instead of module for unit tests
- Prefer using latest available syntax of F# language
- Do not add `Tests` suffix to types with unit tests
- Use `NSubstitute` library to mock interfaces
- Declare and initialize mocks as `type` fields
- Use assertion checks from `FsUnit` and `FsUnit.xUnit` libraries
- Setup mocks before entering `task` computational expression
- Do not add `Mock` suffix to mock variable names
- Do not call `|> ignore` in case if mock is set up inside type `member`
