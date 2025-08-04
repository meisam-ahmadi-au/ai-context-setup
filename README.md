# AI Context Setup Template

A comprehensive template for setting up AI assistant context in any project. This template provides a structured approach for AI assistants to understand, analyze, and work on your codebase effectively.

## Template Structure

### Main Entry Point

- **`ainame.md`** - The main orchestrator file that tells the AI what order to read files and provides context about each component.

### Core Components (`.ainame/` folder)

1. **`codebase-analysis.md`** - Instructions for AI to analyze the codebase and generate an initial assessment
2. **`workflow.md`** - Development workflow and task management process
3. **`testing-strategy.md`** - Testing requirements and standards
4. **`definition-of-done.md`** - Completion criteria for all tasks
5. **`project-context.md`** - Business context and domain knowledge (optional)
6. **`constraints.md`** - Technical, business, and operational constraints (optional)

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

## Customization

This template is designed to be generic and adaptable. Customize it based on:

- Project type (web app, API, mobile app, etc.)
- Technology stack
- Team preferences
- Specific requirements

## Version

Template Version: 1.0
