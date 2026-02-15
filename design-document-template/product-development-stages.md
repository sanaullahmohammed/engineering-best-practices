<!-- Product Development Stages in a Big Company -->

# Product Development Stages

Below outlines four stages of product development. Narrowing in on more and more detailed clarity of the product we're building. The core philosophy of this centers around the idea of achieving alignment across the triad when it's most cheap to do so. It's much easier to change a design document written in english than it is to change a feature or functionality after it has been implemented in code. 

Also core to this is the idea of iterating outcomes. 
We should attempt to achieve high-leve alignment quickly through iterating on the PRFAQ and Solution Spec. Then diving into iterating on the next level of detail with one or more Technical Specifications depending on project size. The size and scope of the Solution Spec should be the entirety of the PRFAQ. The size and scope of the Technical Spec should be roughly equivalent to an EPIC.

This iteration process is key. Humans tend to shy away from diving into detail because it takes work; however, in order for a working implementation to manifest itself the details must be implemented. You do not have one without the other. Often things get misaligned when the triad is not on the same page about these details. The process/framework we outline here hope to achieve alignment on the details quickly and with the least cost. Slow is smooth, smooth is fast. 

```
______________________________________________________________________________
| Product Development                                                         |
|                                                                             |
|          PRFAQ -> Solution Spec -> Technical Spec(s) -> Implementation      |
|                                                                             |
|_____________________________________________________________________________|
```

## PRFAQ (Press Release + FAQ)

- **Outcomes and Benefits** : Clearly articulate the end result and how it benefits the customer
- **Target Audience** : Define who the product is for and the problem it solves
- **Unique Value Proposition** : Highlight what makes the product unique and why it matters
- **Key Features** : Briefly describe the main features and functionalities
- **Market Context** : Provide context about the market needs and how this product fits in
- **Future Vision** : Give a sense of the product's future trajectory and potential expansions

## Solution Spec

- **High-Level Architecture** : Outline the proposed technical architecture and major components
- **Core Functionality** : Define the primary functions the solution will perform
- **Security and Privacy** : Project-wide privacy and security considerations that need to be passed to dependant teams when creating technical specification
- **Scale and Performance** : Outline expected scalability parameters and performance metrics
- **Assumptions** : State the underlying assumptions related to technology, market, and user behaviour
- **Dependency Teams** : Identity internal and external teams the project depends on and the nature of the dependencies
    - **Platform Dependencies** : Special callout of any platform dependencies that there's reasonable expectation of enhancements. Platform components often can be a bottlenect as they serve multiple projects within the company. Calling this out early is important.
- **Risks and Mitigations** : Identify potential risks and how they will be mitigated

## Technical Spec

- **Functional Specifications** : Detailed description of the software's capabililities, features, and behaviour
- **API Shape/Schemas** : Define the API endpoints, request/response structures, and data types
- **Key Data Structures** : Describe the data models and structures that will be used
- **Database Tables** : Outline the databse schema, including tables, columns, indexes, and relationships
- **Assumptions** : List detailed assumptions regarding technology, third-party services, or user interactions
- **Implementation Details** : Provide specifies on algorithms, core logic, state management, and any third-party integrations
- **Security and Privacy** : Address how data security and user privacy will be ensured
- **Deployment Plan** : Outline the steps for deploying the software, including rollback plans

## Implementations / Code

- **Code Quality Standards** : Adhere to coding standards and best practices for readability and maintainability
- **Testing** : Implement unit, integration, and end-to-end tests to ensure functionality and reliability
- **Documentation** : Provide in-code documentation for complex logic, APIs, and setup/configuration instructions
- **Monitoring and Logging** : Set up monitoring and logging to track the application's performance and troubleshoot issues