# Text Editor Enhancement Proposals

Having developed for the third time a text object expansion plugin for yet another vim based environment, I see duplication of design, implementation, and efforts. But why? Lets for a second imagine one backend that could be configured to work as vim or emacs, but sharing logic to jump to function definition in python. This could end the great editor war!

I envision designing javascript interfaces to common components needed by all text editors, with test suites, to assist in developing text editors where their components can be shared, while allowing endless customization. Why javascript? Arguably the most collaberative language available today, and because I dont want to see duplication of efforts occuring in seperate languages.

That being said I do not have sufficient context as to the issues faced and the considerations behind the design choices made in todays leading text editors. I am hoping to foster collaboration between these teams here.

Ultimately I do not want to be a bottleneck, or impose onto the community, beyond an initial draft of the process of collaboration. This is based on Python's PEP standard, however I condensed it to align with the philosophy of TEXEP.

## What is a TEXEP

- Collect community efforts on issues pertaining to building text editors.
- Document design decisions that have gone into text editors that follow TEXEP.
- Can describe requirements of features for text editors or its processes or environment.
- Enable effortless collaboration towards designing text editors.
- Provide concise technical specification and a prototype implementation.
- Build tools and guidelines to assist in developing TEXEP compliant editors.

## Philosophy

- Simple is better than complex.
- Clarity is better than verbosity.
- Practicality beats purity.
- Duplication is the devil.

## Submitting a TEXEP

##### Workflow

- Discuss with the community your idea in a GitHub issue.
  - The issue number will be used as the TEXEP number moving forward.
  - Save time vetting and idea before putting effort into the rest of the process.
  - Is the idea is TEXEP-able?
  - What [type of TEXEP](#types) would you be writing?
  - Why might the proposal be rejected?
  - Is the idea applicable to the community?
  - Is the idea harmonious with the [philosophy of TEXEP](#philosophy).
  - Is there duplication of effort?
- Fork the TEXEP repository and generate a draft proposal.
  - Ensure the draft passes the TEXEP linter.
- Submit as a draft TEXEP via a GitHub pull request for review.
  - Does the structure and formatting meet standards.
  - Contains a single key proposal or new idea.
  - Should not be too small an enhancement.
  - Should not appear too unfocused or too broad.
  - Provides proper motivation.
  - Addresses backwards compatibility.
  - Complies with philosophy of TEXEP.
  - Is technically sound.
- Collaborators will assign its type and status labels to the GitHub issue.
- Author needs to re-ignite discussion to finalize community acceptance.
  - Author must shepherd discussions, build consensus and document dissenting opinions.

##### Types

- Standards Track
  - Design Document
    - Describes a new feature or implementation.
    - Clear and complete with unanimous acceptance.
    - Result in net improvement across design of text editors.
    - Describe interoperability with existing implementations.
  - Reference Implementation
    - Prototype to determine practicality of implementation.
    - Should not complicate existing design unduly.
- Informational
  - Describes design issues or guidelines.
  - Does not represent community consensus or recommendation.
- Process
  - Describes processes surrounding text editing, or changes to process thereof.
  - Similar to Standards Track but apply to areas other than what effects implementation.
  - Procedures, guidelines, changes to the decision-making process, tools or environment, etc.

##### Status

- Draft
  - Pull Request on TEXEP.
  - Satisfies style and format requirements.
- Deferred
  - No progress is being made on the TEXEP.
  - Can be re-assign to draft status by collaborators.
- Approved
  - Merged into TEXEP master.
  - Author accepts responsibly to maintain TEXEP.
  - Open discussion, seeking community consensus.
  - Formalize in documentation efforts.
- Rejected
  - Failed to meet community acceptance.
  - Can not be revised by re-drafting.
- Accepted
  - Has reference implementation.
  - Requires additional community feedback.
- Withdrawn
  - Was accepted.
  - Failed to meet community acceptance.
  - Can not be revised by re-drafting.
- Final
  - No further engagement is needed.
  - No changes are permitted.
  - Can be considered formal documentation of expected behavior.
- Obsolete
  - Was made final.
  - Was superseded by a different TEXEP.
- Active
  - Never meant to be completed.

##### Structure

Standard GitHub markdown `README.md` document within a folder named `./texep/XXX`. Auxiliary files in support of the TEXEP can be included within the folder. Accomplanying GitHub issue which serves as a forum for discussion.

- Meta (maintained in GitHub)
  - Title (<44 chars)
  - TEXEP Number (GitHub issue)
  - Status
  - Type
  - Collaborator (assign to issue)
  - Links
    - Depends (dependant TEXEPs)
    - Replaces (seek to make obsolete TEXEPs)
    - Superseded
- Abstract
  - ~200 word description.
- Specification
  - Describe the syntax and semantics of any new feature.
  - Detail enough to allow competing, interoperable implementations.
- Motivation
  - Explain why the existing language specification is inadequate.
- Rationale
  - Describe what motivated the design.
  - Why particular design decisions were made.
  - What alternate designs were considered.
  - Related work.
  - Evidence of consensus within the community.
  - Discuss important objections or concerns raised.
- Backwards Compatibility
  - Describe incompatibilities and their severity.
  - Proposes to deal with these incompatibilities.
- Reference Implementation
  - Not need to complete before the TEXEP is accepted.
  - Required before making the TEXEP final.
  - Include test code and appropriate documentation.
- Training
  - Documentation to guide community on how to apply the TEXEP.

## Otherwise

TEXEP collaborators don't pass judgment on TEXEPs, acceptance must come from the community. They merely do the administrative & editorial part (which is generally a low volume task).

Please discuss issues or updates to a TEXEP on the original GitHub issue. Without sufficient context you will loose community engagement.

# Next Steps

- Get key community figures to become collaborators.
- Build tools (such as the linter) to assist authors contributing.
- Create TEXEP which details core axioms of text editors.
