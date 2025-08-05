# Post-Subtask Completion Checklist

**MANDATORY**: This checklist MUST be completed after EVERY subtask before proceeding to the next subtask.

## ✅ Completion Steps (Execute in Order)

### 1. Verify Code Functionality

- [ ] Code compiles/runs without errors
- [ ] New functionality works as intended
- [ ] No existing functionality is broken

**Examples:**

- Frontend: Component renders correctly, interactions work
- Backend: API endpoint returns expected response
- Database: Migration runs successfully, queries work
- Configuration: Settings are applied and functional

### 2. Run Relevant Tests

- [ ] Execute tests related to the subtask
- [ ] All tests pass
- [ ] Fix any failing tests before proceeding

**Test Examples by Project Type:**

```bash
# Web Development
npm test -- --testPathPattern=component.test.js
npm run test:unit

# Python
python -m pytest tests/test_feature.py
python -m pytest -k "test_user_auth"

# General
./run_tests.sh
make test
```

### 3. Commit Changes (CRITICAL STEP)

- [ ] Stage all relevant files
- [ ] Create meaningful commit message following `commit-convention.md` format
- [ ] Commit the changes

**Commit Format:** Follow the format specified in `commit-convention.md`:

```
[ainame] type: description
```

**Examples for Subtasks:**

```
[cline] feat: add user authentication middleware
[cline] fix: resolve memory leak in data processing
[cline] test: add unit tests for payment service
[cline] docs: update API documentation for new endpoints
```

**Git Commands:**

```bash
git add .
git commit -m "[ainame] type: your descriptive message here"
```

**⚠️ IMPORTANT**: Review `commit-convention.md` for complete format rules and examples.

### 4. Update Task Tracking

- [ ] Open `tasks-and-subtasks.md`
- [ ] Mark the completed subtask with `[x]` and add completion info
- [ ] Add timestamp and any relevant notes

**Status Update Example:**

```markdown
### Subtasks:

- [x] Subtask 1.1: Create user model (COMPLETE - 2024-01-15 14:30)
- [x] Subtask 1.2: Add validation logic (COMPLETE - 2024-01-15 15:45)
- [ ] Subtask 1.3: Implement API endpoints
```

### 5. Document Any Issues or Notes

- [ ] Record any challenges encountered
- [ ] Note any technical decisions made
- [ ] Update relevant documentation if needed

**Documentation Examples:**

- Code comments for complex logic
- README updates for new dependencies
- API documentation for new endpoints
- Architecture notes for design decisions

## 🚨 CRITICAL REMINDERS

1. **NEVER skip the commit step** - Each subtask MUST have its own commit
2. **NEVER proceed to next subtask** without completing this checklist
3. **NEVER batch multiple subtasks** into a single commit
4. **ALWAYS follow commit-convention.md format** - `[ainame] type: description`

## ⚠️ Common Mistakes to Avoid

- Completing multiple subtasks before committing
- Using vague commit messages
- Skipping tests
- Not updating task tracking
- Proceeding with broken code

## 📋 Quick Verification

Before moving to the next subtask, ask yourself:

- [ ] Did I commit this subtask's changes?
- [ ] Does my commit message follow commit-convention.md format `[ainame] type: description`?
- [ ] Are all tests passing?
- [ ] Is the subtask marked as COMPLETE in tasks-and-subtasks.md?

**If any answer is "No", complete the missing steps before proceeding.**
