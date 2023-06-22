name: Feature request
description: A simple test form to request a feature
title: "[Bug]: "
labels: ["bug", "triage"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for starting this issue!
  - type: input
    id: team_id
    attributes:
      label: Team ID
      description: Please write the id of the team you want to reproduce the pipeline from.
      placeholder: ex. 2T6S
    validations:
      required: true
  - type: dropdown
    id: softwares
    attributes:
      label: Version
      description: What version of our software are you running?
      options:
        - 1.0.2 (Default)
        - 1.0.3 (Edge)
    validations:
      required: true
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://example.com)
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
