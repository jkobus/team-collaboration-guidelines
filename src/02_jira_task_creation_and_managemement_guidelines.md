JIRA Task Creation and Management Guidelines
====

## General Principles

- **Descriptive Titles**: Ensure titles clearly reflect the task content.
- **Changelog Readability**: Craft titles for a diverse audience, including non-technical stakeholders.
- **Task Types**: Use Epics, Stories, Bugs, Tasks and Subtasks appropriately.

## Task Types and Guidelines

### 1. Epics

- **Purpose**: Group large work segments.
- **Title**: Business-oriented and descriptive.
- **Example**: "Integration of Third-Party Payment Gateway" or "Implementation of AI-Based Recommendation Engine".

### 2. Stories (Features)

- **Purpose**: Describe new functionalities.
- **Title Format**: Start with action phrases.
- **SMART Goals**: Specific, Measurable, Achievable, Relevant, Time-bound.
- **Acceptance Criteria**: Define clear completion criteria.
- **Example**: "Develop a user feedback system" with criteria like "Enable feedback on all product pages" and "Collect user ratings and comments".

### 3. Bugs

- **Purpose**: Track and resolve issues.
- **Descriptive Reporting**: Include current behavior vs. expected behavior.
- **Visibility**: Keep on the Kanban board for immediate attention. Do not put them in the Backlog.
- **Example**: "Incorrect tax calculation in checkout process - should align with state tax regulations".

### 4. Tasks (Non-Coding)

- **Purpose**: For non-coding related activities.
- **No PRs**: Typically do not involve coding.
- **Example**: "Organize quarterly team offsite" or "Update internal training materials".

## Task Breakdown and Ownership

- **Breaking Down Large Tasks**: During backlog meetings, large tasks should be broken down into manageable subtasks.
- **Subtask Creation**: For tasks requiring multiple skill sets (e.g., backend and frontend), create separate subtasks detailing each part of the work.
- **Ownership**: Once assigned, a task should remain under the responsibility of the assigned person. Ownership should not change unless absolutely necessary.
- **Collaboration**: If a task requires collaboration, ensure clear communication and division of responsibilities among team members.

## Handling Completed Tasks

- **Finality of Closure**: Once a task is closed, it is considered completed forever.
- **Addressing Post-Completion Issues**: If issues arise related to a task that has already been closed, create a new bug and link it to the original task. Avoid reopening closed tasks. This is important because each task is associated with specific build and deployment stages. Creating a new Pull Request (PR) using the same issue ticket can lead to confusing results and make it more challenging to track the life cycle of that issue.
- **Documentation**: Ensure all relevant information, including the reason for closure, is documented in the task before closing. For example, if it was closed and there was no PR leave some brief note explaining that decision.

## Additional Considerations

- **Regular Updates**: Keep tasks updated with the latest status and information.
- **Documentation and Links**: Attach relevant documents or links for additional context.
- **Offline Updates and Comments**: In the dynamic environment of project management, discussions and decisions often occur outside the JIRA platform, such as during meetings or on communication channels like Slack. To maintain transparency and keep all team members informed, it is crucial to add a comment summarizing any significant offline discussions or decisions related to a task. This practice ensures that everyone has access to the same information and understands the context behind any changes or considerations that have occurred outside of JIRA.
    - **Example**: If a task's scope or priority is adjusted during a team meeting, add a comment on the task detailing the changes and the rationale behind them. Similarly, if a critical decision or insight is shared on Slack that impacts a task, summarize it in a JIRA comment.
- **Feedback and Improvement**: Use feedback from tasks to refine future task creation and management.

## Conclusion

Following these comprehensive guidelines ensures that tasks in JIRA are well-defined, manageable, and transparent. This approach promotes effective project management, clear communication, and accountability within the team.
