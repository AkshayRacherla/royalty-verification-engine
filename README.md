# royalty-verification-engine

This repository contains a prototype of the Decoupled Engine Paradigm for intercompany royalty compliance, designed for the Tresata take-home assignment. Please note that this is a proof-of-concept prototype demonstrating the deterministic mathematical and routing logic, utilizing synthetic data in place of a live LLM extraction endpoint.

**Architecture and Features**
* **Data Layer:** Includes 10 synthetic legal contract extractions and 10 ERP ledger rows to simulate language model outputs.
* **Pre-Math Gatekeeper:** Routes unattached schedules and unsupported jurisdictions directly to human review before any calculation occurs.
* **Deterministic Math:** Employs pure Python arithmetic to compute net revenues, effective rates, and percentage deltas, completely eliminating LLM math hallucinations.
* **Fail-Closed Routing:** Achieves a 10/10 perfect routing score across clean compliance cases, rate/base mismatches, edge cases, and manual ERP accounting corrections.

To view the Python logic, configuration rules, and the final verification dataframe output, open the `Tresata_Assignment.ipynb` file in this repository.
