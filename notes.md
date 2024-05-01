# ![tdd logo](tdd.png) TDD Notes

## What's a test?
A test is an examination of facts that confirms a hypothesis.

Software engineers write tests to evaluate the behavior of programs or components in isolation.

A test is not a proof. We cannot even prove the correctness of a simple program that adds two integers, x and y, for every possible combination of x and y.

## What are some kinds of tests?

### Unit Tests
A unit is the smallest testable part of an application or domain context. A unit might be a function, class, or small set of codependent classes like `LinkedList` and `LinkedListNode`. 

So, a unit test evaluates the behavior of a unit in isolation. Behavior evaluation is the what not the why. I'll cover the why later.

Common unit test tools for unit tests:
- C#: [Xunit](https://xunit.net/)
- Java: [Junit](https://junit.org/)
- Python: [unittest](https://docs.python.org/3/library/unittest.html), [pytest](https://docs.pytest.org/)

### Integration Tests
When we combine [units](#unit-tests) into an interconnected set, we are performing integration. 

So, an integration test evaluates the behavior of, or interactions between, a set of interdependent units.

A common misconception is that integration tests are always applied to deployed system or application. See the section on [end-to-end testing](#end-to-end-tests).

Common unit test tools:
- C#: [Xunit](https://xunit.net/)
- Java: [Junit](https://junit.org/)
- Python: [unittest](https://docs.python.org/3/library/unittest.html), [pytest](https://docs.pytest.org/)

### End-to-End Tests
End-to-end generally means "all aspects of" a system, process, or domain context. Within the context of software testing, end-to-end refers to the execution of a workflow from start to finish.

So, an end-to-end test evaluates a system as it performs a particular workflow. This includes interactions with external systems such as databases and APIs. This can lead to confusion between end-to-end tests and [integration tests](#integration-tests).

- verifies use case scenarios, or workflows, against the deployed application. test tool: Xunit

Common unit test tools:
- C#: [Xunit](https://xunit.net/)
- Java: [Junit](https://junit.org/)
- Python: [unittest](https://docs.python.org/3/library/unittest.html), [pytest](https://docs.pytest.org/)
- Other: New Relic, testRigor, Headspin, Nightwatch, Mabl, Avo Assure, SmartBear, Mobot, Cypress, Testcafe

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
- https://tidyfirst.substack.com/p/canon-tdd
## what is the TDD workflow
## why write tests first
## how does TDD drive decoupling
## what does it mean for a component to be testable? (modular, low coupling, high cohesion (SRP), deterministic behavior, dependency injection)
## why do people resist TDD
## 
