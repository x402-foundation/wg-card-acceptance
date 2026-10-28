# Card Acceptance Working Group Charter

This charter was drafted in the shared x402 working group charters document. From now on, changes to it go through pull requests to this file.

## Purpose

The Card Acceptance Working Group exists to make card payments work over x402 alongside stablecoins. Most buyers and merchants already pay and get paid with cards, and agents acting on their behalf need a way to use those credentials without ever handling raw card data. The group will define how card-based payments fit into the existing x402 model of schemes, networks and facilitators, building on the existing card payment flow. The goal is one open and interoperable approach, so that facilitators, PSPs and sellers don't have to invent their own.

## Strategic Objectives

Define a common way to request, authorize and settle card payments through x402 that any facilitator or PSP can implement.

- Map the landscape: identify the x402 use cases involving cards and cross-pollination (Mastercard Agent Pay, Visa Intelligent Commerce, etc.);
- Define the model: agree on how card payments are represented in x402 and how the card lifecycle maps onto it;
- Adoption and interoperability: validate the approach with more than one card network and PSP before proposing it for the core specification.

## Scope

### In Scope

- How card payments are expressed in x402 payment requirements and payloads, reusing the existing scheme, network and facilitator structure (where possible).
- Use of tokenized or delegated card credentials, so agents and resource servers never handle raw card numbers.
- The card payment lifecycle as it applies to x402: authorization, capture, variable or usage-based amounts.
- Guidance for facilitators and PSPs acting as the card acceptance layer.
- Reference implementations.

### Out of Scope

- Card network rules, fees or interchange, and the internal processes of issuers and acquirers.
- Building, endorsing or certifying any specific PSP, token service or wallet.
- PCI DSS and other compliance obligations of individual implementers. The group might point out where they apply, but won't define them.
- Agent identity in general, tax handling and service discovery, which belong to the [Identity](https://github.com/x402-foundation/wg-identity), [Tax](https://github.com/x402-foundation/wg-tax) and [Domain Discovery](https://github.com/x402-foundation/wg-domain-discovery) working groups.
- Changes to existing stablecoin and onchain schemes, beyond what's needed for cards to sit alongside them.
- Non-card fiat rails such as bank transfers, at least for now.

## Deliverables / Expected Outcomes

### 0 - 3 Months

- Landscape review of existing card programs for agentic payments and how they could map onto x402
- First specification for how card payments are represented in x402 (in progress: [x402-foundation/x402#3707](https://github.com/x402-foundation/x402/pull/3707))

### 3 - 6 Months

- Reference implementation with at least one facilitator or PSP
- Prioritized list of use cases and requirements

### 6 Months+

- Security and compliance considerations for implementers
- Interoperability testing across several card networks and PSPs
- Proposal to the TSC to adopt the specification into x402

## Working Model

### Operating Model

- **Decision-making:** Consensus-driven, with Chair/Co-Chair & TSC representative-led resolution. If consensus cannot be reached, a formal vote will be executed as per the x402 Technical Charter.
- **Work Tracking:** GitHub issues and a project board in the working group repository.
- **Primary Artifacts:** Specification proposals (as pull requests to the [x402 repository](https://github.com/x402-foundation/x402)), reference implementations, test vectors and meeting notes.

## Member Roles

Member roles also decide who gets write access to the working group repository.

- **Participants (Read):** Anyone attending meetings or contributing asynchronously.
- **General Contributors (Triage):** Members focused on project management, issue organization, or those who contribute code and documents infrequently.
- **Core Contributors (Write Access):** Highly active members with a proven track record of substantive, ongoing contributions.
- **Maintainers/Approvers:** Experienced, highly trusted core members who are responsible for the quality, security, and strategic alignment of the working group's outputs.
- **Chairs/Co-Chairs:** Responsible for WG operations, facilitation, and external representation.

| Role | Persona | GH Access | Primary Responsibility |
| :- | :- | :- | :- |
| Participant | Attendees & async followers | Read (Basic access) | Join meetings, open issues, join discussions |
| General Contributor | Periodic contributors | Triage | Organize boards, label issues, submit PRs via forks |
| Core Contributor | Active, ongoing contributors | Write | Push branches directly, review PRs, build solutions |
| Maintainer | Code quality & repo leads | Maintain | Approve & merge PRs, manage releases & standards |
| Chair / Co-Chair | Group Leads | Admin | Group governance, roadmap, admin settings, permissions |
