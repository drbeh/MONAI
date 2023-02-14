name: 🐛 Bug Report
description: Create a report to help us reproduce and fix the bug
labels: 'bug'

body:

- type: markdown
  attributes:
    value: >
      #### Before submitting a bug, please make sure the issue hasn't been already addressed by searching through [the existing and past issues](https://github.com/Project-MONAI/MONAI/issues?q=is%3Aissue+sort%3Acreated-desc+).
- type: textarea
  attributes:
    label: Bug description
    description: |
      Please provide a clear and concise description of what the bug is.
    placeholder: |
      A clear and concise description of what the bug is.
  validations:
    required: true
- type: textarea
  attributes:
    label: Environment
    description: |
      Please run the following and paste the output below.
      ```sh
      python -c 'import monai; monai.config.print_debug_info()'
      ```
  validations:
    required: false
- type: textarea
  attributes:
    label: Code to Reproduce
    description: |
      Please provide a ca minimal example so that we can reproduce the error by running the code.

      It is very important for the snippet to be as succinct (minimal) as possible, so please take time to trim down any irrelevant code to help us debug efficiently.

      Please also paste or describe the results you observe instead of the expected results. If you observe an error, please paste the error message including the **full** traceback of the exception (please wrap error messages in ```` ```triple quotes blocks``` ````.)
      If applicable, add screenshots to help explain your problem.
    placeholder: |
      A minimal example so that we can reproduce the error by running the code.

      ```python
      # Sample code to reproduce the problem
      ```
  validations:
    required: false
- type: markdown
  attributes:
    value: >
      Thanks for contributing to MONAI 🎉!
