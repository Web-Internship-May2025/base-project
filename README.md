# Base Project

## Getting started

In the Base Project, your tasks are in the section [Plan / Issues](https://git.synechron.net/web-internship/may-2025/base-project/-/issues). 

## Issue Boards

In the [Plan / Issue boards](https://git.synechron.net/web-internship/may-2025/base-project/-/boards) there are tasks divided into sections:
- Open
- TO DO
- IN PROGRESS
- REVIEW
- DONE
- Closed

Gitlab [labels](https://git.synechron.net/web-internship/may-2025/base-project/-/labels):
- BUG – that there is an error that needs to be solved.
- FEATURE - labels indicate completely new functionality.
- NON-FUNCTIONAL – that the request is non-functional, mostly some configuration or refactoring.
- ADDITION - addition to already existing functionality.

There are also labels sorted by priority:
- HIGH PRIORITY - task that should have high priority
- MEDIUM PRIORITY - task that should have medium priority
- LOW PRIORITY - task that should have low priority

Other labels are related to the issue boards.

### Open 

In Open you have all unfinished tasks (they have not been assigned to anyone yet). Like product backlog.

A *product backlog* is a prioritized list of work items or features that help you meet product goals and set expectations among teams. It is the single source of work undertaken by the *Scrum Team* and the single source of requirements for the product. 

The product backlog is managed by the *Product Owner* and is never considered complete and is always open to adding, updating, or removing items as the project evolves and business requirements or customer needs change.

### TO DO

In the `TO DO` list are all the unstarted tasks from the current **Sprint** (assigned to each of you).

*Sprint planning* is a crucial event in the Scrum framework that initiates a sprint by defining the work to be performed. 

### IN PROGRESS

In progress, there are tasks whose execution has started. In `IN PROGRESS`, you transfer the tasks you are currently working on and create separate branches for each task from the `development` branch.

Notice:
- If the task has a **FEATURE** label, call the branch `feature/branch_name`.
- If the task has a **BUG** label, call the branch `bugfix/branch_name`.
- If the task has a **NOT FUNCTIONAL** label, call the branch `chore/branch_name`.
- If the task has a **ADDITION** label, call the branch `addition/branch_name`

### REVIEW

In REVIEW there are tasks that have been completed but have not been reviewed and have not been merged to `development` branch.

When you finish the task and when you make a merge request (MR) from your branch to the development branch, mark *Product Owner* as a reviewer (Reviewer option) and transfer the task to the Review list on the board.

When your MR is reviewed, if you need to complete something again or resolve conflicts, move it to `IN PROGRESS`, and when you finish the correction, move it to `REVIEW`. 

MR does not need to be deleted if something needs to be redone on the branch, all commits will just appear at the bottom that you add related to that branch.

### DONE

Once your MR is reviewed and approved, you can merge your branch into `development` (if there are no conflicts). 

Then move the task to the `DONE` tab.

### Closed

When we complete one sprint, i.e. when we pass the *Sprint review* at the end of the sprint, then you move all completed tasks to `Closed` and we together merge the code from `development` to the `main` branch.

## Notice

- When you create branches locally on the git repository, be sure to immediately push it to the global repository as well. And only then start working on that branch.
- Commit mini-units in the code more often.
- Make meaningful comments when you create MR. If it's a frontend task, you can add a screenshot of the frontend part you have done. You can use the template below.
- If you are working on task #34, then you can use the command `$ git commit -m "Put the tag that #34 and write something"` and your issue and your branch will automatically be linked.
- When you create an MR, let me know somewhere in the "Created MR" chat and a link to it.

**MR description template:** 
- Changes in the MR - briefly describe the main changes made in this merge request. 
  - [x] New feature: ..
  - [x] Bug fix: ...
  - [ ] Refactoring: ...
  - [ ] Documentation: ...
  - [ ] Style / UI changes: ... 
- Goal / Motivation: Why was this done? What problem does it solve? [optional]
- How to test: Clear steps to test functionality, UI or logic [optional]
- What to pay attention to during review? Are there any parts that need extra attention: complex logic, new dependencies, etc. [optional]
- Related items: 
  - Issue: #123
  - Documentation: link
  - Design: link
- Additional context / screenshots: Add visuals if UI was changed. 
- Checklist:
  - Code builds locally
  - covered by tests (unit or E2E)
  - documentation updated (if needed)
  - no hardcoded data / sensitive info
  - review requested from team  
