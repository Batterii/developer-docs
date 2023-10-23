# Pull Request Policy for Secure Code

## Overview

This document outlines the policies and best practices for contributing code securely to Vurvey's private repositories. It is mandatory for all team members and contributors to adhere to these guidelines to ensure that the code base remains secure and efficient.

---

## Pre-Requisites

1. **Access Control**: Ensure that you have the necessary permissions to access the private repository and submit a pull request.

2. **Codebase Familiarity**: Familiarize yourself with the codebase and coding standards used within the organization.

3. **Up-to-date Local Repository**: Before creating a new branch, ensure that your local repository is updated to the latest version of the main branch.

4. **Issue Tracker**: All pull requests should be tied to an existing issue in the project's issue tracker.

---

## Steps to Create a Secure Pull Request

### Step 1: Create a New Branch

- Create a new branch locally, branching off the main or development branch. Branch name should have the associate ticket number in the name for linking.

  ```bash
  git checkout -b [branch-name]
  ```

### Step 2: Write Code

- Write the necessary code changes, ensuring to follow secure coding practices like input validation, avoiding hardcoded secrets, etc.

### Step 3: Static Code Analysis

- Run a static code analysis tool to identify any security vulnerabilities or issues in the code.

  ```bash
  npm run lint
  ```

### Step 4: Local Testing

- Perform comprehensive local testing, covering all possible use-cases to ensure that there are no bugs or security vulnerabilities.


  ```bash
  npm run test
  ```

### Step 5: Code Comments and Documentation

- Comment your code adequately and update any relevant documentation.

### Step 6: Commit your Changes

- Use meaningful commit messages.

  ```bash
  git commit -m "Commit message"
  ```

### Step 7: Push to Remote Repository

- Push your changes to the remote repository.

  ```bash
  git push origin [branch-name]
  ```

### Step 8: Create Pull Request

- Go to the GitHub repository and click on "New Pull Request."
- Fill in all the necessary details like the issue it closes, what the PR does, and tag the team members who should review it.

---

## Pull Request Approval Criteria

1. **Code Quality**: The code must adhere to coding standards set by the organization.

2. **Static Analysis**: The code must pass all static analysis checks for security vulnerabilities.

3. **Testing**: The pull request must not break any existing functionality and should pass all automated tests.

4. **Peer Review**: At least one team member who has code review authority role for the repository should review and approve the pull request.

5. **Documentation**: Any changes to the codebase must be reflected in the documentation.

6. **No Secrets**: Ensure that no sensitive data or hardcoded secrets are pushed.

---

## Review Process

1. **Automated Testing**: Automated tests will be run to check for any broken functionality.

2. **Manual Review**: Assigned reviewers will perform a manual code review looking specifically for security vulnerabilities and code quality.

3. **Feedback Loop**: If changes are requested, the contributor must implement these changes and re-submit the pull request.

4. **Merge**: Once all criteria are met and approvals are gathered, the pull request will be merged by a senior team member.

---

## Final Notes

- All pull requests should aim to resolve a single issue. Avoid combining multiple issues into a single pull request unless they are closely related.

- Always mention the issue that the pull request aims to resolve.

- Keep your pull requests as small as possible to make the review process more efficient.

By adhering to this policy, we aim to maintain a secure, efficient, and high-quality codebase. Failure to comply with these guidelines may result in denial of the pull request and further actions as deemed necessary by the organization.
