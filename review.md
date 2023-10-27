# Code Review Rules

Rules for conducting a Code Review.

Code Review is represented as a 5-level pyramid, where the first 2 levels should be automated (but not mandatory).

The lower the level, the more effort will be required to rectify the situation in the future.

* [ ] Code Style
* [ ] Tests
* [ ] Documentation
* [ ] Implementation
* [ ] API

## Code Style

Definition of done:

* [ ] Has the accepted code style been followed (structure, imports, indentation, etc.)?
* [ ] Is the naming consistent?
* [ ] Has the "DRY" principle been followed, or is its violation justified?
* [ ] Is the code readable?

## Tests

Definition of done:

* [ ] Have the tests passed?
* [ ] Have new features been tested to the required extent?
* [ ] Have changes to old features been accompanied by corresponding test changes?
* [ ] Are both main and boundary use cases tested (if necessary)?

## Documentation

Definition of done:

* [ ] Does the architecture in the docs align with reality?
* [ ] Do api in the docs match reality?
* [ ] Does the service's configuration in the docs match reality?
* [ ] Is the "NRF" (Non-Functional Requirements) of the service from the docs fulfilled?
* [ ] Is the observability of the service from the docs ensured?
* [ ] Is the "README" file up to date (or is it unnecessary)?
* [ ] Is the "CHANGELOG" file up to date (or is it unnecessary)?
* [ ] Is the "API" file up to date (or is it unnecessary)?
* [ ] Is the "LICENSES" file up to date (or is it unnecessary)?

## Implementation

Definition of done:

* [ ] Is the logic implemented correctly?
* [ ] Does the architectural style of the project remain intact?
* [ ] Is unnecessary complexity absent?
* [ ] Is the code reliable (no potential issues with asynchronicity, inconsistency, runtime errors)?
* [ ] Are there no performance bottlenecks?
* [ ] Are there no potential security issues?
* [ ] Are there no potential memory leaks?
* [ ] Is logging done correctly?
* [ ] Are there no problems with updated dependencies (libraries, other system components)?

## API

Definition of done:

* [ ] Are specific API standards followed (e.g., Rest, Grpc, etc.)?
* [ ] Are there no logic leaks and dispatching issues in the API?
* [ ] Are breaking changes absent, or have they been coordinated?
* [ ] Is all of the API supported by use cases or test cases?
* [ ] Is the API minimal and sufficient for clients to implement the specified tasks?
* [ ] Is the API fully documented (e.g., XML comments + specification generation for Dotnet)?
* [ ] Is the API atomic within the expected usage scenarios?
* [ ] Does the API allow for future extension (to a reasonable extent) without client-side changes?
