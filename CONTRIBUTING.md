# Contributing to Confluence DC Grafana dashboards

Thank you for considering a contribution to Confluence DC Grafana Dashboards! Pull requests, issues and comments are welcome. For pull requests, please:

* Add tests for new features and bug fixes
* Follow the existing style
* Separate unrelated changes into multiple pull requests

See the existing issues for things to start contributing.

For bigger changes, please make sure you start a discussion first by creating an issue and explaining the intended change.

Atlassian requires contributors to sign a Contributor License Agreement, known as a CLA. This serves as a record stating that the contributor is entitled to contribute the code/documentation/translation to the project and is willing to have it used in distributions and derivative works (or is willing to transfer ownership).

Prior to accepting your contributions we ask that you please follow the appropriate link below to digitally sign the CLA. The Corporate CLA is for those who are contributing as a member of an organization and the individual CLA is for those contributing as an individual.

* [CLA for corporate contributors](https://opensource.atlassian.com/corporate)
* [CLA for individuals](https://opensource.atlassian.com/individual)

## Panel Naming Guidelines

When adding a new panel please ensure the following:
- Title is reasonably formatted
- Has a description
- Placed in appropriate dashboard category (new or existing)

Please follow the existing naming format when naming a title:

`<what is being measured> (<statistical measure (if applicable)> - <cluster wide/per node>)`

Examples:

`DB Core Execution Time (mean - cluster wide)`

`DB Core Execution Time (p99 -  cluster wide)`

`AO Upgrade Tasks - (current - active count)`

If your metric doesn't fit this format, use your best judgement.
