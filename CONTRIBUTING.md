# Contributing to --INSERT PROJ NAME--

## Style

The codebase uses [.net core](https://github.com/dotnet/runtime/blob/master/docs/coding-guidelines/coding-style.md) coding style.

Try to keep lines of code around 100 characters in length or less, though this is not a hard limit.
If you're a few characters over then don't worry too much.

## Pull requests

A single pull request should be submitted for each change. If you're making more than one change,
please submit separate pull requests for each change for easy review. Rebase your changes to make
sense, so a history that looks like:

* Add class A
* Feature A didn't set Foo when Bar was set
* Fix spacing
* Add class B
* Sort using statements

Should be rebased to read:

* Add class A
* Add class B

Again, this makes review much easier.

Please try not to submit pull requests that don't add new features (e.g. moving stuff around)
unless you see something that is obviously wrong or that could be written in a more terse or
idiomatic style. It takes time to review each pull request - time that I'd prefer to spend writing
new features!

Prefer terseness to verbosity but don't try to be too clever.

## Tests

There are one type of tests currently in the codebase; unit tests.

Unit tests should be contained in a class name that mirrors the class being tested with the suffix
-Tests, e.g.

    Arcade.ProjectTracker.Tests.Services.RepoServiceTests

Where Arcade.ProjectTracker.Tests is the name of the project.

Unit test methods should be named in a sentence style, separated by underscores, that describes in
English what the test is testing, e.g.

```csharp
    void Calling_Foo_Should_Increment_Bar()
```

## Code of Conduct

This project has adopted the code of conduct defined by the Contributor Covenant to clarify expected behavior in our community.
For more information see the [Contributor Covenant Code of Conduct](https://dotnetfoundation.org/code-of-conduct)
