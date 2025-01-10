# Commit Message Guide
To maintain professional and consistent commit messages, follow this structure:

Commit Message Structure:

```git
<type>(<scope>): <subject>
```

`<type>`: The type of change (more types listed below).
`<scope>`: The area or module of the project that has been modified (optional, but recommended).
`<subject>`: A brief and clear description of what the change is about.

**Examples**
> feat(user-auth): add password reset feature
> style(ui): adjust button padding for better alignment
> fix(api): resolve bug causing incorrect user data retrieval

## Commit Types and Examples
**feat**: Adding a new feature or functionality to the project.

> Example: Implementing a user login system or adding a contact form.

**fix**: Fixing issues or bugs that affect the functionality of the system.

> Example: Resolving a bug where the login button wasn’t working correctly.

**docs**: Changes related to documentation or explanations in the code.

> Example: Updating the README file to include a new setup process.

**style**: Changes that affect the look or format of the project without altering functionality.

> Example: Adjusting spacing or aligning elements for better readability.

**refactor**: Rewriting or improving the structure of the code without changing its functionality.

> Example: Simplifying a function or improving code readability by renaming variables.

**perf**: Improving the performance or efficiency of the project.

> Example: Optimizing database queries to reduce load times.

**test**: Adding or updating tests to improve test coverage.

> Example: Writing unit tests for a newly implemented feature.

**ci**: Changes related to Continuous Integration (CI) processes.

> Example: Modifying configuration files for automatic deployments.

**build**: Changes related to the build system or dependencies.

> Example: Installing a new package or upgrading a dependency.

**chore**: Miscellaneous tasks that don't fall into the categories of code, tests, or documentation.

> Example: Updating the .gitignore file or cleaning up outdated assets.

**revert**: Reverting changes from a previous commit.

> Example: Undoing a commit that caused a system crash.

### Important Notes:
- feat: When adding a new feature, make sure the related tests are updated.
- fix: Fixes should always be tested and verified to ensure the issue is resolved.
- refactor: Refactor the code for clarity and performance without changing how it works.
- style: Style changes should only focus on improving the appearance or readability of the code.
- perf: Ensure that performance improvements are measurable and significant.
- docs: Documentation updates should be clear and informative.
- test: Tests should improve coverage and ensure the accuracy of your code.
- ci: CI changes should only affect integration or deployment processes.
- build: Make changes to dependencies or build processes without affecting functionality.
- chore: Chores should be non-intrusive and unrelated to the core codebase or tests.
- revert: Use this for undoing changes that caused issues or breakage.
- Commit messages should be simple, clear, and precise so that team members can easily track changes and understand the purpose of each update.


### Best Practices for Using Git and Writing Commit Messages
Commit messages should be simple, clear, and precise so that tracking changes becomes easier for the team.

##### Best Practices for Using Git and Writing Commit Messages
**1. Small and Focused Commits**
Stage and commit each task or change separately. This helps keep the project history clean and traceable.
If you've made many changes, divide related changes into separate commits. 
Example:
- One commit for menu changes.
- One commit for adding a new element.


**2. Write Clear and Specific Commit Messages**

A commit message should:

- Be short and to the point.
- Explain what change was made and why.
- Avoid weak commit messages like "Fix stuff" or "Update files." Good Example:
`fix(header): resolve logo alignment issue in mobile view`

**3. Atomic Commits**

Each commit should represent a small, independent change that works properly if the project is rolled back to that point.
Avoid combining changes for multiple tasks into a single commit.

Bad Example:
Fixing a bug and adding a new feature in one commit.

Good Example:
One commit for fixing a bug and another commit for adding a new feature.

**4. Review Changes Before Committing**

Before committing, use the following command to review your changes:

`git diff --staged`

You can also use Git tools like VSCode or extensions like GitLens.

This helps avoid committing mistakes or unnecessary changes.

**5. Clean and Readable Commits**

Try to avoid committing untested or incomplete code.
Always make sure that the changes you're committing work properly.

**6. Include Documentation in Commits**

If you write a new function, provide necessary explanations in code comments or documentation files.
Make commits related to documentation separately.

**7. Use Branches for Different Tasks**

Create a separate branch for each task or new feature:

`git checkout -b feature/add-new-ad-slot`

After completing the work, merge the branch into the main branch (like main or develop).

Benefits:

- Easier tracking of changes.
- Team members can work in parallel on different sections.

**8. Use Rebase for Cleaner History**

When merging branches, use git rebase instead of git merge to keep the history cleaner. Command:

`git rebase main`

Note: Be careful when using rebase to avoid issues in team collaboration.

**9. Prevent Unnecessary Files from Being Committed**

Define temporary files, caches, and local configurations in .gitignore to prevent them from being committed by mistake.

**10. Use Code Linting Tools**

Use code linting tools like Prettier or ESLint to ensure your code is clean before committing.
You can also set up Git hooks to run these tools before committing.

**11. Use Pull Requests**

Use Pull Requests (PRs) for merging changes. This allows team members to review changes before they are merged.

**12. Practice Using Git**

Git is a powerful tool; frequent use and getting familiar with commands like git stash, git cherry-pick, and git bisect can enhance your efficiency.


These tips will help streamline your team’s workflow, ensure consistency, and make collaboration much more efficient!