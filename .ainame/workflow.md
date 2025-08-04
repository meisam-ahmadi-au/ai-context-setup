# Development Workflow

## Process:

1. Read project-spec.md or goal description
2. Generate tasks-and-subtasks.md with:
   - Main tasks broken into actionable subtasks
   - Dependencies between tasks
   - Estimated complexity (Simple/Medium/Complex)

## Execution Rules:

- Complete one subtask at a time
- Each subtask must result in fully working code
- Commit after each completed subtask with meaningful message
- Mark subtasks as COMPLETE when done
- Test functionality before marking complete

## Commit Message Format:

`[SUBTASK] Brief description of what was implemented`

## Status Tracking:

Update tasks-and-subtasks.md with completion status and timestamps.

## Task File Format:

```markdown
# Tasks and Subtasks

## Task 1: [Task Name]

**Complexity**: [Simple/Medium/Complex]
**Status**: [NOT_STARTED/IN_PROGRESS/COMPLETE]
**Dependencies**: [List any dependencies]

### Subtasks:

- [ ] Subtask 1.1: Description
- [ ] Subtask 1.2: Description
- [x] Subtask 1.3: Description (COMPLETE - timestamp)

## Task 2: [Task Name]

...
```

## Next Steps:

After completing all subtasks, proceed to final review using definition-of-done.md criteria.
