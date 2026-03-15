# lab-agile-planning

A lab repository for exploring GitHub's agile planning features.

---

## GitHub System Overview

### What is a GitHub Issue?

A **GitHub Issue** is a way to track tasks, enhancements, bugs, and questions for a repository. Issues serve as the primary unit of work and communication within a GitHub project.

**Purpose:**
- Track bugs and defects found in the codebase
- Plan and document new features or enhancements
- Ask questions or start discussions about a project
- Assign work to team members
- Link related pull requests to trace changes back to requirements

**Typical Use Cases:**
- **Bug Report:** A user finds unexpected behavior and opens an issue describing the problem, steps to reproduce it, and the expected vs. actual outcome.
- **Feature Request:** A contributor proposes a new feature, explains the motivation, and discusses the approach before any code is written.
- **Task Tracking:** A team breaks down a user story into smaller issues, assigns them to developers, and tracks completion with labels and milestones.
- **Question / Discussion:** Community members ask how to use a specific part of the project, and maintainers or other users respond in the comments.

**Key Features of Issues:**
- **Labels** – Categorize issues (e.g., `bug`, `enhancement`, `documentation`, `help wanted`)
- **Assignees** – Designate who is responsible for resolving the issue
- **Milestones** – Group issues into a target release or sprint
- **Comments** – Allow ongoing discussion and collaboration
- **References** – Link issues to pull requests, commits, or other issues using `#<number>`

---

### What is a GitHub Pull Request (PR)?

A **Pull Request** is a proposal to merge a set of code changes from one branch into another. It is the standard way to contribute code, enabling review and discussion before changes are integrated.

**Purpose:**
- Propose and review code changes before merging them into the main branch
- Facilitate code review and collaboration among team members
- Automatically run CI/CD checks to validate the changes
- Maintain a clear history of why and how changes were made

**Typical Use Cases:**
- A developer finishes work on a feature branch and opens a PR to merge it into `main`.
- A contributor to an open-source project forks the repo, makes changes, and submits a PR to the upstream repository.
- A team uses draft PRs to share work-in-progress and gather early feedback.

**Key Features of Pull Requests:**
- **Code diff view** – Side-by-side comparison of what changed
- **Review requests** – Ask specific team members to review the code
- **Inline comments** – Leave feedback directly on specific lines of code
- **Status checks** – Automated tests and linters that must pass before merging
- **Linked issues** – Closing keywords (e.g., `Closes #42`) automatically close the related issue when the PR is merged

---

### What is a GitHub Project?

A **GitHub Project** is a flexible, customizable planning board that organizes issues, pull requests, and notes into a visual workflow.

**Purpose:**
- Provide a high-level view of work across one or more repositories
- Manage sprints, backlogs, and roadmaps using agile methodologies
- Track the status and priority of all work items in one place

**Typical Use Cases:**
- **Kanban Board:** Columns like `To Do`, `In Progress`, and `Done` give the team a real-time view of progress.
- **Sprint Planning:** A team adds issues to a sprint milestone and uses the project board to track daily progress.
- **Roadmap Planning:** A product team organizes features by quarter to communicate the long-term plan to stakeholders.

**Key Features of Projects:**
- **Custom fields** – Add metadata such as priority, story points, or target date
- **Multiple views** – Switch between Board, Table, and Roadmap layouts
- **Automation** – Automatically move items between columns based on events (e.g., move to "Done" when a PR is merged)
- **Cross-repository** – Aggregate issues and PRs from multiple repositories into a single project

---

### How Issues, Pull Requests, and Projects Work Together

```
Issue (defines the work)
  └──> Pull Request (delivers the code changes)
         └──> Project Board (tracks overall progress)
```

1. A team member creates an **Issue** to describe a bug or feature.
2. A developer branches off, writes the fix or feature, and opens a **Pull Request** referencing the issue.
3. The PR is reviewed, approved, and merged — automatically closing the linked issue.
4. The **Project board** reflects the updated status, giving the whole team visibility into what was completed.