name: 🐛 New Issue
description: Description
title: '[NewIssue]: '
labels:
  - needs triage
body:
  - type: markdown
    attributes:
      value: >
        **Thanks for reporting an issue!** Please make sure you read our [issue
        guidelines](https://github.com/theos/theos/blob/master/.github/CONTRIBUTING.md)
        first, then fill out the fields below.


        If you’re unsure whether the issue you’re having is a bug, you can post
        in [Discussions](https://github.com/theos/theos/discussions) instead.
  - type: textarea
    id: bug-steps
    attributes:
      label: What are the steps to reproduce this issue?
      placeholder: |
        1. Make new project
        2. Run `make package`
        3. …
        4. See error
    validations:
      required: true
  - type: textarea
    id: bug-description
    attributes:
      label: What happens?
      description: A clear and concise description of what the bug is.
    validations:
      required: true
  - type: textarea
    id: bug-expectation
    attributes:
      label: What were you expecting to happen?
      description: A clear and concise description of what was supposed to happen.
    validations:
      required: true
  - type: textarea
    id: bug-logs
    attributes:
      label: Paste any relevant logs, error output, etc.
      description: >
        Please copy and paste any relevant log output. This will be
        automatically formatted into code, so no need for backticks.

        (If it’s long, please paste to https://gist.github.com/ and insert the
        link here.)
      render: shell
  - type: textarea
    id: bug-context
    attributes:
      label: Additional context
      description: Add any other context you can provide about the problem here.
  - type: markdown
    attributes:
      value: >-
        This template was generated with [Issue Forms
        Creator](https://issue-forms-creator.netlify.app)
