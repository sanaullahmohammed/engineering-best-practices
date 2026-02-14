# Solution Spec Template

## Project

- Owner : 
- Status : 
- Jira Theme : 
- PRFAQ (Product Requirements FAQ) :
- UX Spec / Figma : 

## Approvers

- Product Management Owner : [`not yet started` | `approved`]
- Engineering Owner : [`not yet started` | `approved`]
- UX Owner : [`not yet started` | `approved`]
- Dependency Engineering Owner : [`not yet started` | `approved`]
- Architect : [`not yet started` | `approved`]

## Triad members / Contributors

- Product Management : 
- UX : 
- Engineering : 
- Partners : 

## 1. Project Overview

### 1.1 Architecture

Describe 
1. High-Level Architecture : Outline the proposed technical architecture and major components.
2. Core Functionality : Define the primary functions the solution will perform.
3. Key assumptions : Related to technology, market, user behaviour, and dependencies.

This is the core of a Solution Spec. This gives the audience a good design blueprint during the early stage of the SDLC, 
and guide that engineering teams towards the direction when they start the detailed design (as Technical Spec) and implementations. 
We shall avoid overly detailed technical designs here. 

As a general guidance, we target each Solution Spec to have about 30-mins read time.

### 1.2 Product Requirements

Describe
1. Are there any requirements in the PRFAQ and related Jira themes/epics that we need to change based on the solution spec ?
2. Are there any additional edge use case requirements that eng has identified ?

## 2. Architecture Diagrams

To provide a standard architecture diagram. 
The diagram desires reusability with Main app and FedRAMP SCR.

## 3. Standard Topics

There is a list of topics each Solution Spec must cover

### 3.1 Security

- Authentication, Authorization protocols and implementations; 
- RBAC;
- Encryption;
- Secret management;
- Handling of customer data;

### 3.2 Dependencies

- Does this project depend on other engineering deliverables in action or not yet happening ?
- Do we have the committed plan and schedule from the dependent team ?

### 3.3 UI/UX

Is there any engineering design topics which may affect UI and UX ?

### 3.4 Tenancy <!--and MSSP--> Support 

- How the solution design support tenancy. 
- Metering and Billing Design

#### 3.4.1 Tenancy

#### 3.4.2 Metering and Billing

### 3.5 Test Strategy

- Test strategy: 
    - unit, 
    - functional, 
    - integration 
    - testing; 
- production and pre-production testing.

### 3.6 Rollout Strategy

- Engineering estimates of work to be done and rough timelines it will be done in.      
- Engineering execution strategy: Propose if/how we can have a pragmatic execution, say 
producing deliverables in quarterly basis. 
- How does this get exposed to QA, PMs, field, customer ?
- How does this get rolled back ?
- How can I deploy a partially working solution on a dev environment ? 
- How do I release it to Beta customers alongside existing features, EA (Early Access), GA(Global Access).
- Does it introduce any backward compatibility considerations ?
- New releases ?
- Feature toggles ?
- Does it replace certain existing features or implementations ?
- If so, what is the sunset plan of the existing ?

#### 3.6.1 Milestones

#### 3.6.2 Deprecation Plan

### 3.7 Production Readiness

- Does it introduce cloud service dependencies outside company standards ?
- Is the architecture design cloud agnostic (i.e. AWS, GCP, Azure compatible ?)
- FedRAMP related ?
- Performance and scalability considerations ?
- CoGS related ?

#### 3.7.1 Cloud Agnostics

#### 3.7.2 FedRAMP

#### 3.7.3 Performance and Scalability

Describe
1. Design approaches to meet the performance SLO's
2. How we can measure the performance in production as SLA's
3. In case there is any concern or constraint which we project SLO/SLA may not be met, specify explicitly

#### 3.7.4 CoGS

Describe
1. Design approaches to meet the general CoGS expectations
2. If there is any specific concerns which may result higher-than-average company SaaS CoGS concers
3. Any other cost related to 3rd parties (e.g. API calls to 3rd parties which cost us)

#### 3.7.5 Monitoring and Observability

### 3.8 Open Questions, Risks and Issues

This is okay to have questions and issues remaining open in a Solution Spec. 
In fact, a key purpose here is to explore and point out challenges ahead of us, to allo the teams to design solutions int he latter Technical Spec phase.

### 3.9 Standard Adherence

Some checklist styles to ensure the design is aligned with our engineering standards
| Topics | Alignment |
| ------ | -------- |
| Programming Languages | `compliant` `incompliant` | 
| API Protocols | `compliant` `incompliant` | 
| Company approved cloud services for product engineering | `compliant` `incompliant` | 
| FE Standards (UQL, GraphQL, Gateway, Localization, WCAG) | |
| Operatoinal support (zero down time, horizontal scalability) | |

### 3.10 Permissions and Licensing 

## 4. References

## Template Revision

| Revision | Date | Description | 
| ---- | --- | ---- | 
| v0.1 | 14/02/2026 | Intial Draft |
