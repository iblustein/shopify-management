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

Follow the [Conventional Commits](https://www.conventionalcommits.org/) standard:

```
<type>(scope): <short description>
```

**Types:** `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `style`

**Examples:**
```
feat(cart): add discount code validation
fix(checkout): resolve payment gateway timeout
docs(readme): update setup instructions
chore(deps): bump shopify-api version to 7.1.0
```

**Rules:**
- Use the imperative mood ("add" not "added")
- Keep the subject line under 72 characters
- Reference the task ID in the body when applicable: `Closes task dev-003`

---

## Pull Request Process

1. **Create a branch** from `main` using the naming convention above.
2. **Write your code** and commit with clear messages.
3. **Open a PR** targeting `main` with:
   - A clear title following the commit format
   - A description of what was changed and why
   - Reference to the task ID (e.g. `Task: dev-003`)
4. **Request a review** — at least one approval is required before merging.
5. **Do not merge your own PR** unless explicitly approved.
6. **Delete the branch** after the PR is merged.

### PR Checklist
- [ ] Branch is up to date with `main`
- [ ] Code has been tested locally
- [ ] No console logs or debug code left in
- [ ] Relevant documentation updated if needed

---

## General Guidelines

- Keep PRs small and focused — one task per PR.
- If you're unsure about an approach, open a draft PR and ask for feedback early.
- Agent-generated code must be reviewed by a human before merging to `main`.

---

_Maintained by the Stoked Dev Team. Questions? Reach out to Neo (Main Agent)._
