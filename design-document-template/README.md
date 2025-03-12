# \<Feature Name\> Design Doc

Author(s) : \<1 or more authors\>  
Date : \<Start Doc Date\>  
Reviewers : \<List of reviewers\>
Status : \<Draft | Under Review | Approved\>

## Objective

\<This is the goal of the document. The reviewers approve the doc based on this goal. The goal is to outline the design review process and create a template for the document\>

## Background

\<If the problem space is new, please add a brief background section on the current state or add links to the feature spec or ADO (Azure DevOps)\>

## Design

\<Please cover your design as part of this section. It should be concise while elaborating on any aspects that need clarification, especially when certain assumptions/choices are being made.\>

## Future Investments

\<List the areas identified as part of this design that need further investigation and state whether it blocks the implementation of the current design. Also add relative priorities, ownership, and impact as part of this design.

Refer [Timelines, Estimates and Unknowns](#timelines) & [Future Investments](#future)\>

## Timelines and Estimates

\<Add timelines, preferable owners, and estimates for the tasks identified as part of this design. Also create relevant Epic -\> Feature -\> User Story -\> Tasks in ADO whenever the design is approved.

Refer [Timelines, Estimates and Unknowns](#timelines)\>

## Conclusion

\<Conclusion for the proposal and the final design decision\/choice which was approved\>

## Appendix

#### Related Docs and Links

\<Add links to references, etc.\>

#### Recording Link

\<Add recording link of the design review meeting here, if conducted\>

# Design Review Process and Additional Details

## Overview

The goal of this section is to cover the design process for features where there are more “Knowns” than “Unknowns”. Features that have lot of “Unknowns” might go through iterations of experimentation before we can get to the design stage. Here “Knowns” and “Unknowns” refer to technical “Knowns” and “Unknowns” and experimentation refers to technical feasibility and technical approach analysis. There may be product “Unknowns” or experimentations required. That will still require a design document if the feature needs to be deployed to production.

## Reviewers

### List of reviewers

Please include Gautam, Rohith, PMs, devs or SMEs, based on relevance to this feature.

### Reviewers’ responsibility

Review the document based on the goals, and suggest improvements, changes & concerns. This is a loop with the authors till the state is “Approved”. The expectation from reviewers is to review the document at least 1 day before the design review meeting, but the sooner is better. No design document should be sitting for more than 1 week before sending out feedback.

### Review Flow

1. Reviewer Notified (Doc is in Under Review State)
2. Reviewer suggests edits, requests more information, and adds comments/concerns.
3. Document Updated
   • Design Review meeting scheduled (if needed)
   • Reviewer marks as “Good to Go” and the document is moved to Approved state

## Status

1. **Draft**: Authors are working on the design. It is not open for review.
2. **Under Review**: The reviewers have been added and requested to review the contents of the document.
3. **Approved**: Once approved by reviewers and the document has been updated to reflect the changes, the document can be marked as reviewed.

## Timelines, Estimates & Unknowns <a id="timelines"></a>

One of the goals of the design process is to ensure that the design clearly covers the points mentioned below, discussed with the above group of reviewers, and agreed upon.

- Design for functional requirements. Impact on extensibility & maintainability.
- Impact on non-functional requirements such as cogs, scalability, availability, etc. are known and are in line with our longer-term goals and commitments.

If these are clearly covered in the design and agreed upon, we can estimate the time and developer bandwidth it would take to deliver the feature.

Estimating will help with the predictability of feature delivery timelines. Capturing estimations here will help us to improve our estimation skills as we can revisit them and compare them against the actual time taken.

For this process to be effective, it’s important that there are as few “Unknowns” as possible. The goal for the design process is to get to a stage where there is clarity on what we need to code to meet the above functional and non-functional requirements. At the same time, there may be areas that require further investigation and experimentation before we can have this confidence. Hence one important goal is to cover such “Unknowns” and estimate for “Knowns”. If the “Unknowns” are not a blocker for parts of the requirements, we can start implementing those while we have an ETA to get back with the design for the “Unknowns” after completing experiments. We will continue to work on the “Unknowns” only if the solution to them is deemed necessary to meet the requirements.

## Future Investments <a id="future"></a>

There would be “Unknowns” that we don’t know how to solve for or don’t want to solve for at that time. However, if there is a consensus that they are required for the medium to longer term, we add those as items that need future investment and cover the details we know so far. This can happen if the feature itself is experimental (from a product standpoint) and does not impact the medium to longer-term goals we have on non-functional characteristics of the product or if we need to deliver the feature within a strict timeline, but we need to look at this for the next release. We need to have an agreement on what kind of future investment it is and when do we need to start looking at it.
