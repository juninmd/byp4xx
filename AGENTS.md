# AGENTS.md File Guidelines

These guidelines are designed to ensure the consistent, high-quality, and maintainable development of all AI coding agents within this repository. Adherence to these principles is mandatory for all development activities.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent should have a single, well-defined purpose. Avoid creating overly complex agents with multiple functions that serve similar tasks.
*   **Component Reusability:** Components should be designed to be reusable across multiple agents where appropriate.
*   **Code Patterns:** Utilize established code patterns and libraries to minimize redundant code.
*   **Abstraction:**  Implement abstractions where possible to avoid exposing implementation details.
*   **Documentation:**  Document complex logic and high-level concepts clearly.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimize Complexity:** Keep agent code concise and easy to understand. Avoid unnecessary layers or dependencies.
*   **Readability:** Use clear and descriptive variable names, comments, and formatting.
*   **Logical Flow:** Ensure the code follows a logical and sequential flow.
*   **Avoid Over-Engineering:** Resist the temptation to over-optimize for minor gains; prioritize clarity and maintainability.

## 3. SOLID Principles

*   **Single Responsibility:**  Each class/component should have only one reason to change.
*   **Open/Closed Principle:**  The system should be extensible without modifying the existing code. (Limited reliance on external libraries).
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:** Each interface should have a limited scope.
*   **Dependency Inversion Principle:**  High-level modules should not depend on low-level modules; they should be treated as abstractions.

## 4. YAGNI (You Aren't Gonna Need It)

*   **Avoid Unnecessary Features:**  Do not implement functionality that is not currently required.  Refactor to remove unused code.
*   **Focus on Core Functionality:** Prioritize the implementation of essential agent behaviors.
*   **"Write Once, Use Anywhere":** Strive to create agents with a limited set of core functionalities.

## 5. Development Workflow & Best Practices

*   **Code Reviews:** All code changes must be reviewed by at least one other developer.
*   **Unit Tests:**  All agents must have comprehensive unit tests covering all critical functionality. Tests are required for every major function.
*   **Test Coverage:**  Aim for at least 80% test coverage. Test suite is documented with a clear indicator of testing target.
*   **Dependency Management:** Utilize a dependency management system (e.g., `pip`) with strict versioning.  Dependencies must be declared in `requirements.txt`.
*   **Error Handling:** Implement robust error handling to prevent unexpected crashes.
*   **Logging:**  Include appropriate logging for debugging and monitoring.
*   **Documentation:**  Update documentation to reflect changes and usage.
*   **Version Control:** Use Git for version control and follow established branching strategies.
*   **Commit Messages:**  Write clear and concise commit messages explaining the purpose of each change.

## 6. File Length & Structure

*   **Maximum Code Length:** 180 lines of code per file.
*   **File Organization:**  Follow a consistent directory structure.
*   **Component Structure:** Each agent should ideally be organized into distinct components or modules with well-defined responsibilities.
*   **Modular Design:** Break down complex agents into smaller, manageable modules.
*   **Documentation Comments:** All functions and classes should have detailed documentation comments.

## 7.  Testing & Validation

*   **Test Driven Development (TDD):**  Consider TDD principles for the development of new agents.
*   **Automated Tests:**  Implement automated tests to validate agent functionality.
*   **Regression Testing:**  Ensure that new changes do not break existing functionality.

## 8.  Data Management (Mocking)**

*   **Mocking:**  All data and interactions must be mocked for testing.  No real data should be used.
*   **Interface Driven Testing:**  Focus testing on the *interface* of agents, not their internal state.
*   **Test Data:** Use test data that is clearly defined and independent of the real application.

## 9.  Code Standards

*   Follow established coding standards (e.g., PEP 8 for Python).
*   Use consistent naming conventions.
*   Write clear and concise code.

This document provides a foundational set of guidelines.  Regularly review and refine these guidelines as needed to maintain the quality and maintainability of the AGENTS.md repository.