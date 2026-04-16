/src
├── domain
│   ├── models          # Core business logic
│   ├── value-objects   # Objects with internal logic (e.g., Email)
│   ├── repositories    # Abstract interfaces (ports)
│   └── services        # Domain services
│
├── application
│   ├── use-cases       # Orchestrate domain operations
│   └── dto             # Data Transfer Objects
│
├── infrastructure
│   ├── db              # Database connection and models
│   ├── repositories    # Concrete implementations of interfaces
│   └── services        # External services (e.g., email)
│
├── interfaces
│   └── http
│       ├── routes      # API endpoints definitions
│       ├── controllers # Handle requests and call use-cases
│       └── middlewares # Express middlewares
│
├── shared              # Common types, errors, helpers
└── index.ts            # Application entry point

This project follows a Hexagonal Architecture (Ports & Adapters) approach.

The goal is to separate business logic from external concerns such as databases,
frameworks or APIs, making the application more maintainable, testable and scalable.

- Domain: Core business rules and logic
- Application: Use cases that coordinate domain behavior
- Infrastructure: External implementations (database, services)
- Interfaces: Entry points (HTTP controllers, routes, middlewares)

- ## 🚀 Backend API – Node.js & TypeScript

Scalable REST API built with Node.js and TypeScript using Hexagonal Architecture.
Focused on clean code, modular design and real-world backend practices.
