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
- **MANDATORY**: Execute `post-subtask-completion.md` checklist after EVERY subtask
- **MANDATORY**: Execute `post-task-completion.md` checklist after EVERY task
- Commit after each completed subtask with meaningful message
- Mark subtasks as COMPLETE when done
- Test functionality before marking complete

## Critical Workflow Steps:

### After Each Subtask:

1. **STOP** - Do not proceed to next subtask
2. **EXECUTE** the complete `post-subtask-completion.md` checklist
3. **VERIFY** code works and tests pass
4. **COMMIT** following `commit-convention.md` format
5. **UPDATE** tasks-and-subtasks.md with completion status
6. Only then proceed to next subtask

### After Each Task:

1. **STOP** - Do not proceed to next task
2. **EXECUTE** the complete `post-task-completion.md` checklist
3. **VERIFY** all subtasks are complete and committed
4. **TEST** comprehensive task functionality
5. **UPDATE** task status and documentation
6. Only then proceed to next task

## Commit Message Format:

Follow the format specified in `commit-convention.md`:

`[ainame] type: description`

**Examples:**

- `[cline] feat: add user authentication system`
- `[cline] fix: resolve memory leak in data processing`
- `[cline] test: add unit tests for payment service`

## Status Tracking:

Update tasks-and-subtasks.md with completion status and timestamps.

## Task File Format:

```markdown
# Tasks and Subtasks

## Task 1: User Authentication System

**Complexity**: Medium
**Status**: IN_PROGRESS
**Dependencies**: Database setup, User model

### Subtasks:

- [x] Subtask 1.1: Create user model with validation (COMPLETE - 2024-01-15 14:30)
- [x] Subtask 1.2: Add password hashing logic (COMPLETE - 2024-01-15 15:45)
- [ ] Subtask 1.3: Implement login API endpoint
- [ ] Subtask 1.4: Add JWT token generation
- [ ] Subtask 1.5: Create authentication middleware

## Task 2: Payment Processing

**Complexity**: Complex
**Status**: NOT_STARTED
**Dependencies**: User Authentication System, Stripe API setup

### Subtasks:

- [ ] Subtask 2.1: Set up Stripe SDK integration
- [ ] Subtask 2.2: Create payment model
- [ ] Subtask 2.3: Implement payment processing endpoint
- [ ] Subtask 2.4: Add payment confirmation logic
- [ ] Subtask 2.5: Create payment history view

## Task 3: Frontend User Interface

**Complexity**: Simple
**Status**: NOT_STARTED
**Dependencies**: User Authentication System

### Subtasks:

- [ ] Subtask 3.1: Create login form component
- [ ] Subtask 3.2: Add registration form component
- [ ] Subtask 3.3: Implement dashboard layout
- [ ] Subtask 3.4: Add responsive design styles
```

### Example Commit History for Task 1:

```
[cline] feat: create user model with validation
[cline] feat: add password hashing logic
[cline] feat: implement login API endpoint
[cline] feat: add JWT token generation
[cline] feat: create authentication middleware
[cline] feat: complete user authentication system (optional summary)
```

## Next Steps:

After completing all subtasks, proceed to final review using definition-of-done.md criteria.
