# Project Portfolio: Applied Cybersecurity Risk Management

This repo contains documentation from two projects. These projects demonstrate the application of core cybersecurity principles in both regular IT environments and specialized Industrial Control Systems (ICS). The goal is to make the textbook concepts applicable to real-world scenarios.

---

## 1. Cybersecurity Risk Assessment Project (IT Context)

This project focused on GRC (Governance, Risk, and Compliance) principles within the fictional tech startup "Innovate Solutions." The primary objective was to identify the most significant cyber threats, prioritize them logically, and create a clear, business-focused mitigation plan.

### Skills & Activities

The standard GRC process was executed, with an emphasis on practical outcomes:

*   **Risk Management:** A structured approach was used to identify, analyze, and prioritize risks. Standardization was achieved using a scoring matrix (Likelihood x Impact).
*   **Framework Application:** The **NIST Cybersecurity Framework (CSF)** was applied. High-level NIST categories were translated into actionable steps for the business.
*   **Documentation:** Professional reports and detailed risk registers were created for management review.
*   **Problem Solving:** Abstract threats were converted into specific controls, such as mandatory **MFA**, setting up **Firewalls**, and running targeted **Security Training**.

### Deliverables

The reports generated are available in the repo:

*   **`Company-Profile.md`**: Business and asset context.
*   **`Risk-Register-Matrix.xlsx`**: Spreadsheet used for scoring risks.
*   **`Risk-Assessment-Report-Final.pdf`**: The formal report for the C-suite.
*   **`Security-Controls-Recommendation.pdf`**: The actionable mitigation plan.

---

## 2. Domain 1 Report: ICS Security Principles & Risk Management (OT Context)

This second part contrasts with the IT project, focusing on high-stakes Industrial Control Systems (OT). A key takeaway was recognizing that OT priorities differ significantly from IT.

### The Real-World CIA Triad in OT

Priorities change when protecting a power plant or factory:

*   **Availability is paramount.** System downtime can have serious consequences. Security solutions must not interfere with safety or uptime. Resilience is the primary focus.
*   **Integrity is crucial.** Accurate process data prevents accidents. Physical safety is the priority, not just data accuracy.
*   **Confidentiality is third.** It's important for intellectual property, but physical safety comes first in the control room.

### Applied Risk Management: Theory to Practice

The goal was to bridge the gap between theory and practical application:

*   **Active Risk Assessment:** Real risks, such as unsecured USB drives and unpatched legacy systems, were examined.
*   **Smart Risk Treatment:** Sometimes, a *calculated* risk must be accepted on an old, essential system. The approach taken was to mitigate this by isolating it from the network.
*   **Hands-On Controls:** Firewalls were configured specifically for industrial protocols (like Modbus/TCP) to ensure only essential traffic passes through.
*   **Framework Expertise:** The **ISA/IEC 62443** and **NIST SP 800-82** standards, built for this environment, were heavily used.

---

## Conclusion & Next Steps

These projects provided a solid understanding of cybersecurity governance, risk management, and the distinction between IT and OT security.

The current focus is expanding this by writing sample code to automate some recommended controls, such as a script to audit user permissions as part of an access control review process.

