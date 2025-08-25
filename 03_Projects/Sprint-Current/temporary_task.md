# API Error Handling Refactoring Request

## Context

In my current API implementation (specifically within the `run.py` file), the codebase contains a large number of `try`/`except` blocks that are repetitively embedded within individual functions. This redundancy is leading to cluttered logic and reduced readability.

## Objective

I would like to refactor the error-handling approach to follow a more structured and maintainable practice. Specifically, I aim to:

- Remove the excessive `try`/`except` blocks from within the internal business logic functions.
- Centralize error handling at higher levels—particularly at the API route (endpoint) level and the application-level middleware (if applicable).
- Ensure that all raised exceptions from lower-level functions are appropriately handled and logged at the API layer.
- Preserve clarity, traceability, and graceful error reporting for clients.

## Request

Please assist me in the following:

1. Identify a clean and scalable error-handling strategy that adheres to best practices for modern API development (e.g., using FastAPI or Flask).
2. Provide guidance or patterns for refactoring the existing functions to remove internal `try`/`except` blocks.
3. Offer a modular structure for centralized exception handling, including custom exception classes and reusable error response utilities.
4. If applicable, update or suggest modifications to `run.py` that reflect this refactored design.

The goal is to achieve a more maintainable, robust, and professional API architecture by simplifying error-handling responsibilities and ensuring separation of concerns.
