name: Bug Report
description: Create a report to help us improve
title: ''
labels: [bug, triage]
assignees: ''
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: Also tell us, what did you expect to happen?
      placeholder: Tell us what you see!
      value: "A bug happened!"
    validations:
      required: true
  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots
      description: If applicable, add screenshots to help explain your problem.
      placeholder: You can add images by clicking on the top button
    validations:
      required: false
  - type: dropdown
    id: version
    attributes:
      label: Version
      description: What version of Iris are you running?
      options:
        - Iris & Sodium 1.16
        - Iris Standalone 1.16
        - Iris Standalone Beta 1.17
    validations:
      required: true
  - type: input
    id: os
    attributes:
      label: What is your OS?
      description: Please write your Operating System
      placeholder: ex: Windows 10
    validations:
      required: true
  - type: input
    id: gpu
    attributes:
      label: What is your GPU?
      description: Please write the vendor and model of your GPU
      placeholder: ex: Nvidia GeForce 1060
    validations:
      required: true
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: Please copy and paste any relevant log output. This will be automatically formatted into code, so no need for backticks.
      render: shell
  - type: textarea
    id: additional-context
    attributes:
      label: Additional context
      description: Add any other context about the problem here.
    validations:
      required: false
  - type: checkboxes
    id: search-first
    attributes:
      label: Have you searched for similar issues?
      description: Before submitting this issue, please check there are no similar issues on (the issue tracker)[https://github.com/IrisShaders/Iris/issues]
      options:
        - label: I have searched for similar issues and found none
          required: true
