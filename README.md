# Assignment 3: Managing a Software Project with GitLab and GitHub

This repository is a practical checklist for creating and managing a small
software project with GitLab or GitHub. Complete the tasks below in order and
use the repository history and project settings as evidence of completion.

## Learning objectives

- Create and manage a project on GitLab or GitHub.
- Use milestones to track project progress.
- Create, assign, and complete issues.
- Clone a repository and contribute through branches and pull/merge requests.
- Manage collaborator access using the least privilege required.

## 1. Create the project

1. Create a new repository named
   `Assignment-3-Managing-a-Software-Project-with-GitLab-GitHub`.
2. Keep the repository private unless the instructor requires it to be public.
3. Add this README and make an initial commit on the default branch.
4. Clone the repository locally:

   ```bash
   git clone <repository-url>
   cd Assignment-3-Managing-a-Software-Project-with-GitLab-GitHub
   ```

## 2. Plan with a milestone

Create a milestone named **Assignment complete** with a due date agreed with
the instructor. Use the milestone description to record the assignment goal.
Close the milestone only after all linked issues are complete.

Suggested milestone checklist:

- [ ] Project created and initialized
- [ ] Issues created and assigned
- [ ] Branch contribution merged
- [ ] Collaborator access reviewed

## 3. Create and assign issues

Create one issue for each deliverable and assign it to the person responsible.
Add the **Assignment complete** milestone to every issue.

Suggested issues:

| Issue | Acceptance criteria |
| --- | --- |
| Set up the project | Repository exists, has a default branch, and contains a README. |
| Track work with a milestone | Milestone exists and all assignment issues are linked to it. |
| Contribute through a branch | A feature branch and pull/merge request are reviewed and merged. |
| Review collaborator access | Collaborators have only the permissions they need. |

Use labels such as `documentation`, `workflow`, and `access` to make issues
easy to filter. Close an issue only when its acceptance criteria are met.

## 4. Contribute through a branch

Do not make the assignment change directly on the default branch. Create a
descriptive branch, commit a focused change, and open a pull request (GitHub)
or merge request (GitLab):

```bash
git switch -c docs/project-workflow
# make and review a focused change
git add README.md
git commit -m "Document project management workflow"
git push -u origin docs/project-workflow
```

Request a review, address feedback, and merge the request only after the
checks pass. Reference the related issue in the request (for example,
`Closes #1`) so the platform records the connection between the work and the
issue.

## 5. Manage collaborator access

Open the repository's **Settings → Collaborators** (GitHub) or
**Project information → Members** (GitLab) page. Invite each contributor using
their platform username and grant the lowest role that permits their task:

- **Read/Reporter** for people who only need to view the project.
- **Triage/Developer** for people who need to manage issues or contribute code.
- **Maintain/Maintainer** only for trusted project managers who must change
  repository settings.

Review the access list before submitting the assignment, remove unnecessary
invitations, and never commit passwords, access tokens, or other credentials.

## Evidence of completion

Submit links or screenshots showing the project repository, the completed
milestone, assigned issues, the merged pull/merge request, and the final
collaborator list. Keep the repository history intact so the commits and
branch workflow can be verified.