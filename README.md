# AI Context Setup Template

A comprehensive template for setting up AI assistant context in any project. This template provides a structured approach for AI assistants to understand, analyze, and work on your codebase effectively.

## Template Structure

### Main Entry Point

- **`ainame.md`** - The main orchestrator file that tells the AI what order to read files and provides context about each component.

### Core Components (`.ainame/` folder)

1. **`codebase-analysis.md`** - Instructions for AI to analyze the codebase and verify runtime functionality
2. **`workflow.md`** - Development workflow and task management process
3. **`commit-convention.md`** - AI name + semantic commit message standards and examples
4. **`post-subtask-completion.md`** - MANDATORY checklist after each subtask (prevents commit skipping)
5. **`post-task-completion.md`** - MANDATORY checklist after each task (ensures comprehensive completion)
6. **`testing-strategy.md`** - Testing requirements and standards
7. **`definition-of-done.md`** - Completion criteria for all tasks
8. **`project-context.md`** - Business context and domain knowledge (optional)
9. **`constraints.md`** - Technical, business, and operational constraints (optional)

## How to Use This Template

1. **Copy the template** to your new project directory
2. **Customize `ainame.md`** with your project-specific information:
   - Fill in `[TO BE FILLED]` placeholders
   - Update the project type
   - Add any project-specific notes
3. **Configure the components** in `.ainame/` folder:
   - Update testing frameworks and requirements
   - Customize definition of done criteria
   - Fill in project context and constraints
4. **Let the AI read** `ainame.md` to start the structured workflow

## AI Workflow Process

1. **Analysis Phase**: AI reads `codebase-analysis.md` and generates `initial-assessment.md`
2. **Planning Phase**: AI reads project specs and creates `tasks-and-subtasks.md`
3. **Development Phase**: AI executes tasks following the workflow rules
4. **Quality Assurance**: Each subtask is tested and meets definition of done criteria
5. **Completion**: All tasks completed with meaningful commits and working code

## Key Features

- **Structured Approach**: Clear reading order and process flow
- **Quality Focus**: Built-in testing and definition of done
- **Flexibility**: Optional components for different project needs
- **Trackability**: Progress tracking and meaningful commit messages
- **Modularity**: Easy to customize for specific project types

## Template Benefits

- Ensures AI understands your project before starting work
- Maintains code quality through testing and review criteria
- Provides consistent workflow across different projects
- Enables incremental development with working code at each step
- Facilitates clear communication between human and AI
- **Prevents commit confusion** with explicit post-completion checklists
- **Enforces proper git workflow** with mandatory commit-per-subtask rules

## Commit Workflow Enforcement

This template specifically addresses common AI assistant mistakes:

### The Problem

AI assistants often:

- Complete multiple subtasks without committing
- Commit only after entire tasks instead of individual subtasks
- Use vague commit messages
- Skip the commit step entirely

### The Solution

- **`post-subtask-completion.md`**: Mandatory checklist that MUST be executed after every subtask
- **`post-task-completion.md`**: Comprehensive checklist for task completion
- **Explicit examples**: Good vs bad commit messages with concrete examples
- **STOP commands**: Clear instructions to halt progress until commits are made
- **Verification steps**: Checklists to ensure commits happened correctly

### Expected Commit Pattern

```
[cline] feat: create user model with validation
[cline] feat: add password hashing logic
[cline] feat: implement login API endpoint
[cline] feat: add JWT token generation
[cline] feat: create authentication middleware
[cline] feat: complete user authentication system (optional)
```

This ensures every piece of working code is committed individually, making it easy to track progress and roll back specific changes if needed.

## Customization

This template is designed to be generic and adaptable. Customize it based on:

- Project type (web app, API, mobile app, etc.)
- Technology stack
- Team preferences
- Specific requirements

## Version

Template Version: 1.0
