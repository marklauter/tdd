# Software Test Notes
Real programmers build the test harness as they code. Testing is not a separate task. 

## What's a test?
A test is an examination of facts that confirms a hypothesis.

Software engineers write tests to evaluate the behavior of programs or components in isolation.

A test is not a proof. We cannot even prove the correctness of a simple program that adds two integers, x and y, for every possible combination of x and y.

## What are some kinds of tests?

### Unit Tests
A unit is the smallest testable part of an application or domain context. A unit might be a function, class, or small set of codependent classes like `LinkedList` and `LinkedListNode`. 

So, a unit test evaluates the behavior of a unit in isolation. Behavior evaluation is the what not the why. I'll cover the why later.

### Integration Tests
When we combine [units](#unit-tests) into an interconnected set, we are performing integration. 

So, an integration test evaluates the behavior of, or interactions between, a set of interdependent units.

A common misconception is that integration tests are always applied to a deployed system or application. See the section on [end-to-end testing](#end-to-end-tests).

### End-to-End Tests
End-to-end generally means "all aspects of" a system, process, or domain context. Within the context of software testing, end-to-end refers to the execution of a workflow from start to finish.

So, an end-to-end test evaluates a system as it performs a particular workflow. This includes interactions with external systems such as databases and APIs. 

But don't confuse end-to-end tests with [integration tests](#integration-tests). The difference is the scope. While an end-to-end test encompasses the entirety of the system and its dependencies, the scope of integration tests is limited to a smaller set of interconnected components.

### Static Code Analysis
Static code analysis tools review source code for correctness, best practices, anti-patterns, code smells, and vulnerabilities. Advanced analysis was once the domain of dedicated tools like SonarQube. Today compilers, like Roslyn, are full-featured static analyzers. The first guardian of quality is the compiler or linter. A professional does not tolerate hints nor warnings.

IDEs manage static analysis through the [editorconfig file](https://editorconfig.org/). 

### Dynamic Analysis
Dynamic analysis refers to the study of a system under real-world conditions. The goal is to find runtime issues like memory leaks, performance issues, and reliability issues. Analyzers review logs and metrics collected during profiling. Specialized tools perform stress testing, fuzz testing, simulate system outages, etc. Dynamic analysis is related to the field of system reliability engineering (SRE).

### Common Test Tools
- For unit tests and integration tests
  - C#: [Xunit](https://xunit.net/)
  - Java: [Junit](https://junit.org/)
  - Python: [unittest](https://docs.python.org/3/library/unittest.html), [pytest](https://docs.pytest.org/)
- For E2E tests
  - any of the unit test or integration test tools
  - New Relic
  - testRigor
  - Headspin
  - Nightwatch
  - Mabl
  - Avo Assure
  - SmartBear
  - Mobot
  - Cypress
  - Testcafe

## what's the point of /unit/ testing
- wip
  
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
