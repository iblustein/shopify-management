# Contributing to Shopify Management

Thank you for contributing to this project! Please follow the guidelines below to keep our codebase consistent and our workflow smooth.

---

## Branch Naming Conventions

All branches should follow this naming pattern:

```
<type>/<short-description>
```

### Types
| Type | Purpose |
|------|---------|
| `feature/` | New features or enhancements |
| `fix/` | Bug fixes |
| `task/` | Agent-assigned or operational tasks |
| `chore/` | Maintenance, dependency updates, tooling |
| `hotfix/` | Urgent production fixes |

### Examples
- `feature/add-product-sync`
- `fix/order-webhook-handler`
- `task/dev-003-contributing-md`
- `hotfix/checkout-crash`

> ⚠️ Never commit directly to `main`. All changes must go through a pull request.

---

## Commit Message Format

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>(<scope>): <short description>

[optional body]

[optional footer]
```

### Types
- `feat` – a new feature
- `fix` – a bug fix
- `docs` – documentation changes only
- `chore` – maintenance tasks (no production code change)
- `refactor` – code restructuring without feature changes
- `test` – adding or updating tests
- `ci` – CI/CD pipeline changes

### Examples
```
feat(products): add bulk sync from Shopify Admin API
fix(webhooks): handle missing order ID in payload
docs(readme): update setup instructions
chore(deps): upgrade @shopify/api to v9
```

**Rules:**
- Use imperative mood: "add feature" not "added feature"
- Keep the subject line under 72 characters
- Reference task IDs in the footer when applicable: `Refs: dev-003`

---

## Pull Request Process

1. **Branch from `main`** — always create your branch off the latest `main`.
2. **Keep PRs focused** — one PR per feature, fix, or task. Avoid unrelated changes.
3. **Write a clear PR title** — follow the same format as commit messages.
4. **Fill out the PR description** with:
   - What changed and why
   - How to test it
   - Any relevant screenshots or logs
5. **Self-review your diff** before requesting a review.
6. **Request at least one reviewer** before merging.
7. **Squash and merge** is preferred to keep the history clean.
8. **Delete the branch** after the PR is merged.

### PR Title Examples
- `feat(orders): add retry logic for failed webhooks`
- `fix(auth): resolve token expiry on long sessions`
- `task(dev-003): add CONTRIBUTING.md`

---

## Agent-Assigned Tasks (A2A)

When tasks are assigned via the A2A system:
- Tasks land in `tasks/dev/<task-id>.md`
- Create a branch named `task/<task-id>-<short-description>`
- Write results to `tasks/results/<task-id>-result.md`
- Update the task file Status from `pending` to `completed`
- Never deploy — open a PR and notify the DevOps agent

---

## Questions?

Open an issue or reach out to the team via the project's internal channels.
