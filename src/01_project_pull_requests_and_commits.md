Project Pull Request and Commit Guidelines
====

## Introduction
This document outlines the guidelines for creating Pull Requests (PRs) and working with commits in our project.  
Adherence to these guidelines ensures smooth integration with our automation systems, easier code management, and a cleaner, more understandable git history.

## Key Principles
- **Clear Reference**: Each PR and commit must reference a JIRA issue for traceability and automation purposes.
- **Squash Commits**: PRs should contain a single, squashed commit to simplify rollbacks and git log readability.
- **Avoid Merge Commits**: Directly integrate changes with the development branch without merge commits.
- **Descriptive Commit Messages**: Avoid vague descriptions to maintain clarity in the project's history.

## Guidelines
1. Pull Request Title  
   **Format**: Use the JIRA issue number and title.  
   **Example**: For a JIRA issue titled "Add ability to create a FooBar" with the issue number FD-123, the PR title should be: `FD-123 Add ability to create a FooBar`.

2. Commit Description  
   **Format**: Follow the same format as the PR title.  
   **Example**: `FD-123 Add ability to create a FooBar`

3. Squashing Commits  
   **Single Commit per PR**: Ensure only one commit per PR. If multiple people work on a PR, each contributor should squash their commits.  
   **Timing**: Perform squashing at the end of the review process to avoid conflicts.  
   **Group Squashing**: If commits are from different contributors, squash only your commits to avoid changing the authorship of others' work.  

4. Avoiding Merge Commits  
   Ensure your commit is on top of the latest development branch.  
   Use rebase instead of merge to integrate changes from the development branch.  

5. Automation and JIRA Reference  
   The automation system relies on valid JIRA task references in PRs and commits.  
   Ensure each commit message includes the JIRA issue number.  

6. Rollback and Git Log Clarity  
   A single commit per feature or fix simplifies the process of rolling back changes.  
   A clean git log with well-documented commits aids in project understanding and tracking.

7. Commit Message Quality  
   Avoid non-descriptive commit messages like "fix", "another fix", or "fixing bug".  
   Ensure each commit message clearly describes the change or addition.  

8. PR Regex Pattern  
   **Regex Pattern**: `^(\w+-\d+)\s(.+)$`  
   This pattern ensures the PR title starts with the JIRA issue number (e.g., `FD-123`), followed by a space and a descriptive title.  

## Examples:

### Good Commit Message
- FD-123 Implement X to improve Y
- FD-123 Add ability to create a FooBar
- FD-123 FooBar returned wrong results upon query
- FD-123 Update FooBar creation to use new API

Clearly references the JIRA issue and describes the change.

### Bad Commit Message
- fix bug
- another fix
- fixing bug
- FD-123
- changed docs line
- merged changes

Lacks a JIRA reference and/or does not describe the change.

## Conclusion
Adhering to these guidelines ensures a streamlined workflow, facilitates automation, and maintains a clear and useful project history.  
It is crucial for all team members to follow these practices for efficient and effective project management.