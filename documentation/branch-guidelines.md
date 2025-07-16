# 🌿 Branch Naming Guideline (Feature-Based with Jira)

This guideline outlines the branch naming convention for a Git repository using a **feature-based workflow** and **Jira** for planning.

---

## 🔧 General Format

```
<type>/<jira-key>-<short-description>
```

Example:
```
feature/APP-123-login-form
```

---

## 📂 Branch Types

| Type       | Description                                 |
|------------|---------------------------------------------|
| `feature`  | New features                                |
| `bugfix`   | Bug fixes                                   |
| `hotfix`   | Critical fixes for production               |
| `chore`    | Technical tasks (e.g., refactoring)         |
| `test`     | Experimental or prototype branches          |
| `release`  | Release preparation branches                |

---

## 🧩 Jira Key

- Use the **issue key** from Jira, e.g., `APP-123`
- Helps link the code to the ticket

---

## ✍️ Description

- Use lowercase only
- Separate words with hyphens `-`
- No spaces or special characters
- Keep it short and meaningful

---

## ✅ Examples

```bash
feature/APP-123-login-form
bugfix/APP-456-api-error-on-submit
hotfix/APP-789-critical-crash-on-load
chore/APP-321-update-dependencies
test/APP-999-experiment-new-layout
release/APP-1000-v2.1.0
```

---

## 🧠 Best Practices

- **Consistency** is more important than perfection
- Branches should be created from the correct base (`main` or `dev`)
- The Jira ticket and branch should clearly correspond
- Avoid overly long names (max. 5–6 words)

