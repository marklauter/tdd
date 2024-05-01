# notes
## what is a test

## what are the kinds of tests
- unit - verifies individual code components, like classes or functions, in isolation.
- integration - verifies interaction between sets of components
- end-to-end - verifies use case scenarios, or workflows, against the deployed application 
- static code analysis (hints, warnings, sonar) - scan code on merge for best practice conformity, secrets, maintainability - like LINT or Sonar Cube
- dynamic code analysis - ex OWASP ZAP. purpose identify runtime issues like memory leaks and performance issues.

## what's the point of /unit/ testing
- what's a unit? the smallest possible source code block that provides value within a domain context
  
important
- rapid feedback loop - iteration over the domain context helps developer learn - faster is better
- isolation - components tested in an isolated and controlled environment have well defined behaviors which can be trusted when integrated
- improved compont and domain context design - due to testable components exhibiting "testablity" (modular, low coupling, high cohesion (SRP), deterministic behavior, dependency injection)
  - ^ low coupling and high cohesion required for testable code are desirable attributes for domain context simulation
  - testability forces the design of well defined, deterministic behaviors
- unit tests are the canon demo and documentation of the source code's behavior

lucky sideeffect
- validation / quality assurance
- early detection
- regression prevention



## what is test driven development (TDD)
## what is the TDD workflow
## why write tests first
## how does TDD drive decoupling
## what does it mean for a component to be testable? (modular, low coupling, high cohesion (SRP), deterministic behavior, dependency injection)
## why do people resist TDD
## 
