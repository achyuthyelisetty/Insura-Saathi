# Insura-Saathi

### AI-Powered Health Insurance Coverage Auditor

**Insura-Saathi** is an AI-assisted solution designed to help families
understand potential out-of-pocket expenses during ICU stays, before the
final hospital bill arrives.

When families are already under pressure, interpreting lengthy insurance
policies and hospital bills can be difficult. Insura-Saathi aims to turn
these documents into a clearer, evidence-backed estimate of potential
insurance coverage shortfalls.

## The Problem

Insurance policies may include room-rent caps, sub-limits, co-payments,
exclusions, and proportionate deductions. These conditions can affect
the amount an insurer may cover, yet families may struggle to estimate
their financial exposure during treatment.

## The Solution

Insura-Saathi brings policy and bill analysis into one guided workflow:

1.  Upload a health insurance policy and an interim hospital bill.
2.  Extract relevant policy clauses and bill details using OCR and
    AI-assisted document retrieval.
3.  Structure and validate extracted information.
4.  Apply a deterministic rules engine to calculate the estimated
    coverage.
5.  Present the estimate with supporting evidence, or flag the case for
    manual review.

## Key Features

-   **Document extraction:** Reads policy documents and hospital bills,
    including scanned files.
-   **Policy clause interpretation:** Identifies relevant limits,
    co-payments, exclusions, and deduction conditions.
-   **Deterministic calculations:** Uses code for financial calculations
    rather than relying on free-form AI output.
-   **Evidence-backed results:** Connects interpretations to source
    information from the policy.
-   **Human-in-the-loop review:** Escalates ambiguous clauses, missing
    pages, conflicting information, and unsupported outputs.
-   **Privacy-conscious MVP design:** Proposes session-only document
    handling by default and explicit consent before processing.

## Technology and Architecture

-   **OCR:** Text extraction from scanned documents
-   **Retrieval-Augmented Generation (RAG):** Context-grounded retrieval
    and interpretation of policy clauses
-   **Python:** Coverage calculation and validation logic
-   **Streamlit:** Planned prototype interface
-   **Structured JSON:** Validated hand-off between AI interpretation
    and the calculation engine

**Design principle:** AI reads and interprets; deterministic code
calculates; a human verifies.

## Evaluation Plan

The project defines a proposed evaluation framework using **60 synthetic
policy-and-bill scenarios** covering room-rent caps, sub-limits,
proportionate deductions, co-payments, ambiguous clauses, missing
information, and bill-format variations.

  Evaluation metric                                    Proposed target
  -------------------------------------------------- -----------------
  Field-level extraction accuracy                                ≥ 90%
  Clause interpretation accuracy                                 ≥ 85%
  Calculation accuracy against manual calculations                100%
  Unsupported-claim rate                                         \< 5%
  Correct escalation rate                                        ≥ 90%

These are **proposed targets, not confirmed results**. Evaluation
results must be measured before making claims about system performance.

## Safety and Limitations

-   Estimates are informational and do not guarantee insurer
    reimbursement.
-   Ambiguous or incomplete information should be escalated rather than
    guessed.
-   Human verification is required before an estimate is relied upon.
-   The MVP scope is limited to one policy and one bill per audit.
-   Broader user research, willingness-to-pay validation, and testing on
    real-world documents remain necessary.

## Current Status

The project is a capstone concept with a prototype and evaluation plan.
The performance targets above remain pending validation.

## Future Scope

-   Evaluate extraction and interpretation on diverse, real-world
    document formats with appropriate consent.
-   Improve handling of missing pages, endorsements, and conflicting
    clauses.
-   Conduct supervised pilot testing with human review of every
    estimate.
-   Validate user needs and pricing assumptions through further
    research.

## Project Team and Academic Context

Developed as part of the **Agentic AI Product Management Capstone at IIM
Sambalpur**.

## Author

**Achyuth Athreya Yelisetty**\
LinkedIn: linkedin.com/in/achyuth-yelisetty

------------------------------------------------------------------------

*Insura-Saathi: Your insurance companion when every rupee matters.*
