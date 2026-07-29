What is Jenkins?

Jenkins is an open-source automation server used to automate software development tasks such as building, testing, and deploying applications. It is one of the most widely used CI/CD tools.

Jenkins monitors your source code repository (such as GitHub). When new code is pushed, it can automatically start a pipeline to build, test, and deploy the application.


How Jenkins Works

Developer writes code
        │
        ▼
Git Commit
        │
        ▼
Push to GitHub
        │
        ▼
Jenkins detects changes
        │
        ▼
Starts Pipeline
        │
        ├── Checkout Code
        ├── Build
        ├── Run Tests
        ├── SonarQube Analysis
        ├── Create Artifact
        └── Deploy


Jenkins Architecture
           Jenkins Server
          (Master/Controller)
                  │
      ┌───────────┴───────────┐
      │                       │
Agent 1                  Agent 2
(Build Java)           (Run Tests)

