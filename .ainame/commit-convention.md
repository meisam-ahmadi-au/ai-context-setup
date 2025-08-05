# Commit Convention

## Format

All commits MUST follow this format:

```
[ainame] type: description
```

### Components:

- **`[ainame]`**: The name of the AI assistant making the commit (e.g., `[cline]`, `[claude]`, `[gemini]`)
- **`type`**: Semantic commit type (see types below)
- **`description`**: Brief, clear description of the change

## Semantic Commit Types

### Primary Types:

- **`feat`**: New features or functionality
- **`fix`**: Bug fixes
- **`docs`**: Documentation changes only
- **`test`**: Adding, updating, or fixing tests
- **`refactor`**: Code refactoring without changing functionality
- **`style`**: Code style changes (formatting, semicolons, etc.)
- **`chore`**: Maintenance tasks, dependency updates, build changes

### Additional Types:

- **`perf`**: Performance improvements
- **`security`**: Security-related changes
- **`config`**: Configuration file changes
- **`deps`**: Dependency updates
- **`revert`**: Reverting previous commits

## Examples

### ✅ GOOD Examples:

```
[cline] feat: add user authentication system
[cline] fix: resolve memory leak in data processing
[cline] docs: update API documentation for new endpoints
[cline] test: add unit tests for payment service
[cline] refactor: optimize database query performance
[cline] style: fix indentation and remove trailing spaces
[cline] chore: update dependencies to latest versions
[cline] config: add environment variables for production
[cline] security: implement input validation for user forms
[cline] perf: optimize image loading with lazy loading
```

### ❌ BAD Examples:

```
updated code
fixes
changes
working on feature
almost done
temp commit
[cline] stuff
[cline] fix
feat: something
cline: added feature
```

## Subtask vs Task Commits

### Subtask Commits (Most Common):

Use the standard format for individual subtasks:

```
[cline] feat: create user registration form
[cline] test: add validation tests for user model
[cline] fix: handle edge case in password validation
```

### Task Summary Commits (Optional):

For optional task-level summary commits:

```
[cline] feat: complete user authentication system
[cline] feat: implement payment processing with Stripe
[cline] refactor: migrate database from SQLite to PostgreSQL
```

## Special Cases

### Breaking Changes:

Add `!` after the type for breaking changes:

```
[cline] feat!: change API response format for user endpoints
[cline] refactor!: restructure database schema
```

### Multi-line Descriptions:

For complex changes, use body text:

```
[cline] feat: implement advanced search functionality

- Add full-text search with indexing
- Support for filters and sorting
- Pagination for large result sets
- Search history and saved searches
```

### Co-authored Commits:

When working with human developers:

```
[cline] feat: implement real-time chat system

Co-authored-by: Developer Name <dev@example.com>
```

## Commit Message Guidelines

### Description Rules:

- Use imperative mood ("add" not "added" or "adds")
- Start with lowercase letter
- No period at the end
- Keep under 50 characters for the description
- Be specific and descriptive

### Good Description Patterns:

- `add [feature/component]`
- `implement [functionality]`
- `fix [specific issue]`
- `update [what was updated]`
- `remove [what was removed]`
- `refactor [what was refactored]`

## Project-Specific Customization

### AI Name Configuration:

Update the AI name based on which assistant is being used:

- `[cline]` for Cline
- `[claude]` for Claude
- `[gemini]` for Gemini
- `[gpt]` for ChatGPT
- `[copilot]` for GitHub Copilot

### Custom Types:

Projects may add specific types:

- `[cline] migration: add user roles table`
- `[cline] seed: add sample data for development`
- `[cline] deploy: update production configuration`

## Verification Checklist

Before committing, ensure:

- [ ] AI name is in square brackets
- [ ] Semantic type is correct and lowercase
- [ ] Description is clear and specific
- [ ] Format follows: `[ainame] type: description`
- [ ] Description uses imperative mood
- [ ] No typos or grammatical errors

## Integration with Workflow

This convention integrates with:

- **post-subtask-completion.md**: References this file for commit format
- **post-task-completion.md**: Uses this format for task summary commits
- **workflow.md**: Enforces this convention throughout development
- **Git history**: Creates clean, searchable commit history

## Benefits

- **Clear Attribution**: Know which AI made which changes
- **Professional Standards**: Follows industry-standard semantic commits
- **Searchable History**: Easy to find specific types of changes
- **Automated Tools**: Compatible with changelog generators and CI/CD
- **Team Integration**: Works well with human developer workflows
