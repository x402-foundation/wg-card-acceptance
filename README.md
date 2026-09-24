# Card Acceptance Working Group

The **Card Acceptance Working Group** standardizes traditional payment card network schemes (credit, debit, and prepaid), virtual account numbers (VANs), EMVCo network tokenization, and acquirer settlement within the x402 (RFC 9110 HTTP 402) protocol framework.

As autonomous AI agents, automated services, and programmatic clients transact across the web, card acceptance bridges traditional financial infrastructure (Visa, Mastercard, American Express, Discover) with machine-to-machine HTTP payments.

## Leadership & Governance

* **Chair**: Stefano Amorelli
* **Co-Chair**: Carson Roscoe
* **Operating Model**: All work is conducted openly under the Linux Foundation Antitrust Policy and Apache-2.0 license.

## Goals

The primary goals of the Card Acceptance Working Group are:

1. **Standardize HTTP 402 Card Payment Schemes**: Define normative wire formats and JSON schemas for card-based payment challenges in the `accepts` array of an HTTP 402 response (e.g., `scheme: "card"`, accepted networks, acquirer parameters, and currency capabilities).
2. **Autonomous Agent Tokenization & Non-Interactive Flows**: Specify secure delegation patterns for automated agent checkout using EMVCo Network Tokens and merchant-bound virtual cards, ensuring Primary Account Numbers (PAN) and sensitive cardholder data never enter LLM prompt context or agent logs.
3. **Interactive Step-Up & Strong Customer Authentication (SCA)**: Define standardized challenge-response extensions for 3-D Secure (3DS 2.x), biometric passkeys (WebAuthn), and issuer step-up authentication when human-in-the-loop authorization is required.
4. **Hardware-Isolated Execution & Compliance Boundaries**: Codify security guidelines for card credential management inside hardware-isolated execution environments (Confidential Computing / Enclaves, Apple Secure Enclave) to satisfy PCI-DSS and enterprise security standards.
5. **Cross-Working Group Interoperability**: Harmonize card acceptance semantics with Domain Discovery (host/route capability advertisement), Identity (agent credential mandates), and Tax (verifiable receipts and merchant compliance).

## Anticipated Deliverables

* **Specification**: *x402 Scheme Specification: Card & Network Token Acceptance*.
* **JSON Schema**: Normative schemas for card requirements, payment authorization payloads, and settlement receipts.
* **Reference Vectors**: Test suites for non-interactive token payments and 3DS step-up challenge flows.
* **Implementation Guide**: Best practices for PCI-DSS compliance and hardware enclave credential isolation for autonomous agents.

## Meetings

Bi-weekly on Tuesdays (alternating with Identity WG)  
10:00 AM CT | 11:00 AM ET | 8:00 AM PT | 4:00 PM BST | 11:00 PM SGT

A schedule of public meetings and calendar links can be found on the [x402 Community Calendar](https://x402.org/get-involved/#calendar).

### Resources

- Past meeting notes and agendas are available [online](https://docs.google.com/document/d/1SPlTQYm_ysVsF_I_TmhwAfQiSjapSaUmSov9-RoMLRI/edit?tab=t.0).
- Recordings of public meetings are accessible through the LFX platform.

## Communication Channels

- **Public Slack**: [#wg-card-acceptance](https://x402workspace.slack.com/archives/C0BH70XKYHL)
- **Mailing List**: [Card-Acceptance-Working-Group@lists.x402.org](mailto:Card-Acceptance-Working-Group@lists.x402.org) (Subscribe at [lists.x402.org](https://lists.x402.org/g/Card-Acceptance-Working-Group))
