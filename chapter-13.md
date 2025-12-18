# CHAPTER 13: Software Engineering & Design

Engineering principles applied to software development.

## 1. The Software Development Life Cycle (SDLC)
The process of planning, creating, testing, and deploying information systems.
- **Models**: Waterfall (sequential), Agile (iterative, flexible), DevOps (continuous integration and deployment).
- **Phases**: Requirement Analysis, Design, Implementation, Testing, Deployment, Maintenance.

## 2. Version Control (Git) and Branching
- **Git**: A distributed version control system. Tracks changes in source code.
- **Branching**: Creating a separate line of development. Allows features to be developed in isolation (Feature Branch Workflow) and merged back (Pull Request) after review.

## 3. Design Patterns (Singleton, Factory, Observer)
Reusable solutions to common problems.
- **Singleton**: Ensures a class has only one instance (e.g., Database connection).
- **Factory**: Creates objects without specifying the exact class to be created.
- **Observer**: A subscription mechanism where objects (observers) are notified of state changes in a subject (e.g., Event listeners).

## 4. Testing Strategies (Unit, Integration, E2E)
- **Unit Testing**: Testing individual components/functions in isolation. Fast, granular.
- **Integration Testing**: Testing how different modules work together.
- **End-to-End (E2E) Testing**: Testing the complete flow of the application from the user's perspective (e.g., using Selenium/Cypress). Slower, brittle, but validates real-world scenarios.
