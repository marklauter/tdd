# ![tdd logo](tdd.png) TDD Notes

## What's a test?
A test is an examination of facts that confirms a hypothesis.

Software engineers write tests to evaluate the behavior of programs or components in isolation.

A test is not a proof. We cannot even prove the correctness of a simple program that adds two integers, x and y, for every possible combination of x and y.

## What are some kinds of tests?

### Unit Tests
- validate behavior of individual code components, like classes or functions, in isolation.
- test tools
  - C# Xunit
  - Java Junit
  - Python unittest, pytest

### Integration Test
- verifies interaction between sets of components. test tool: Xunit

### End-to-End Tests
- verifies use case scenarios, or workflows, against the deployed application. test tool: Xunit

### Static Code Analysis
- (hints, warnings, sonar)
- scan code on merge for best practice conformity, secrets, maintainability.
- test tool: LINT, Sonar, Roslyn. related: editorconfig

### Dynamic Analysis 
- purpose identify runtime issues like memory leaks and performance issues.
- test tool: OWASP ZAP, etc

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
