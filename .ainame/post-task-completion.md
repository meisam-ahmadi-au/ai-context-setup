# Post-Task Completion Checklist

**MANDATORY**: This checklist MUST be completed after ALL subtasks of a task are finished before proceeding to the next task.

## ✅ Task Completion Steps (Execute in Order)

### 1. Verify All Subtasks Are Complete

- [ ] Check that all subtasks are marked with `[x]` in tasks-and-subtasks.md
- [ ] Confirm each subtask has a completion timestamp
- [ ] Ensure each subtask was committed individually

**Verification Example:**

```markdown
## Task 1: User Authentication System

**Status**: COMPLETE
**Dependencies**: None

### Subtasks:

- [x] Subtask 1.1: Create user model (COMPLETE - 2024-01-15 14:30)
- [x] Subtask 1.2: Add validation logic (COMPLETE - 2024-01-15 15:45)
- [x] Subtask 1.3: Implement API endpoints (COMPLETE - 2024-01-15 16:20)
- [x] Subtask 1.4: Add authentication middleware (COMPLETE - 2024-01-15 17:10)
```

### 2. Run Comprehensive Task Tests

- [ ] Execute full test suite for the completed task
- [ ] Run integration tests if applicable
- [ ] Verify end-to-end functionality

**Test Examples by Task Type:**

```bash
# Full Feature Testing
npm run test:feature -- auth
npm run test:integration

# API Task Testing
npm run test:api
curl -X POST http://localhost:3000/api/auth/login

# Frontend Task Testing
npm run test:e2e
npm run test:component -- UserAuth

# Database Task Testing
npm run test:db
python manage.py test auth_app

# Full Application Testing
npm run test:all
make test-full
./run_integration_tests.sh
```

### 3. Verify Against Definition of Done

- [ ] Review definition-of-done.md criteria
- [ ] Confirm all acceptance criteria are met
- [ ] Check code quality standards

**Definition of Done Examples:**

- [ ] Code is properly documented
- [ ] All tests pass (unit, integration, e2e)
- [ ] Code follows project style guidelines
- [ ] No security vulnerabilities introduced
- [ ] Performance requirements met
- [ ] Accessibility standards followed (if applicable)

### 4. Update Task Status

- [ ] Mark task as COMPLETE in tasks-and-subtasks.md
- [ ] Add completion timestamp
- [ ] Update overall project progress

**Status Update Example:**

```markdown
## Task 1: User Authentication System

**Complexity**: Medium
**Status**: COMPLETE - 2024-01-15 17:30
**Dependencies**: None
**Completion Notes**: All authentication features implemented and tested. Ready for production deployment.
```

### 5. Optional: Create Task Summary Commit

- [ ] Consider creating a summary commit for the entire task (optional)
- [ ] Follow `commit-convention.md` format: `[ainame] type: description`

**Task Summary Commit Examples:**

✅ **GOOD Task Summary Examples:**

```
[cline] feat: complete user authentication system with login/logout/registration
[cline] feat: implement payment processing with Stripe integration
[cline] style: add responsive design for mobile devices
[cline] refactor: complete database migration to PostgreSQL
[cline] feat: implement real-time chat functionality with WebSockets
```

**Git Commands for Task Summary:**

```bash
# Optional - only if you want a summary commit
git add .
git commit -m "[ainame] type: brief description of completed task"
```

**⚠️ IMPORTANT**: Review `commit-convention.md` for complete format rules and semantic types.

### 6. Update Documentation

- [ ] Update project README if needed
- [ ] Update API documentation
- [ ] Update user documentation
- [ ] Update deployment notes

**Documentation Update Examples:**

**README Updates:**

```markdown
## Features

- ✅ User Authentication (Login, Registration, Password Reset)
- ✅ Payment Processing (Stripe Integration)
- 🔄 Real-time Chat (In Progress)
- ⏳ Admin Dashboard (Planned)
```

**API Documentation:**

```markdown
## Authentication Endpoints

### POST /api/auth/login

- Description: Authenticate user and return JWT token
- Body: { email, password }
- Response: { token, user }
```

### 7. Prepare for Next Task

- [ ] Review dependencies for upcoming tasks
- [ ] Ensure current task doesn't block future work
- [ ] Clean up any temporary files or code

## 🚨 CRITICAL REMINDERS

1. **NEVER mark a task complete** if any subtask is incomplete
2. **ALWAYS verify end-to-end functionality** before marking complete
3. **ENSURE all individual subtask commits exist** - don't rely only on task summary
4. **UPDATE project documentation** to reflect new functionality

## ⚠️ Common Mistakes to Avoid

- Marking task complete with incomplete subtasks
- Skipping comprehensive testing
- Not updating documentation
- Forgetting to verify definition of done criteria
- Not checking task dependencies

## 📋 Task Completion Verification

Before proceeding to the next task, confirm:

- [ ] All subtasks are marked COMPLETE with timestamps
- [ ] Each subtask has its own commit following commit-convention.md format
- [ ] Comprehensive tests pass
- [ ] Definition of done criteria met
- [ ] Task marked COMPLETE in tasks-and-subtasks.md
- [ ] Documentation updated
- [ ] No blocking issues for future tasks

## 🎯 Success Indicators

A task is truly complete when:

- ✅ All functionality works as specified
- ✅ All tests pass consistently
- ✅ Code meets quality standards
- ✅ Documentation is up to date
- ✅ Ready for production deployment (if applicable)

**If any indicator is missing, address it before proceeding to the next task.**
