# Codebase Analysis Instructions

## Task:

Analyze the entire codebase and generate `initial-assessment.md` with:

### Required Analysis:

- Project structure and organization
- Technology stack identification
- Key components and their relationships
- Entry points and main workflows
- Dependencies and external integrations
- Code patterns and conventions used
- **Runtime verification** (NEW)

### Runtime Verification:

Before proceeding with development, verify if the application can run:

#### Build/Compile Check:

- Attempt to build/compile the project
- Document any build errors or warnings
- Identify missing build tools or configurations

#### Dependency Health:

- Check if all dependencies can be installed
- Verify version compatibility
- Document any missing or conflicting dependencies

#### Application Startup:

- Attempt to start/run the application
- Test basic functionality if possible
- Document startup errors or issues

#### Environment Requirements:

- Identify required environment variables
- Document system requirements (Node.js version, Python version, etc.)
- List required external services (databases, APIs, etc.)

### Runtime Verification Examples by Project Type:

#### Node.js/React Projects:

```bash
# Check dependencies
npm install
# or
yarn install

# Build the project
npm run build
# or
yarn build

# Start the application
npm start
# or
yarn start

# Test basic functionality
curl http://localhost:3000
```

#### Python Projects:

```bash
# Check dependencies
pip install -r requirements.txt
# or
poetry install

# Run the application
python app.py
# or
python manage.py runserver
# or
flask run

# Test basic functionality
curl http://localhost:5000
```

#### Java/Spring Projects:

```bash
# Build with Maven
mvn clean install

# Build with Gradle
./gradlew build

# Run the application
java -jar target/app.jar
# or
mvn spring-boot:run

# Test basic functionality
curl http://localhost:8080
```

#### PHP Projects:

```bash
# Install dependencies
composer install

# Start development server
php -S localhost:8000
# or
php artisan serve (Laravel)

# Test basic functionality
curl http://localhost:8000
```

### Assessment Format:

- **Understanding**: What this project does
- **Architecture**: How it's structured
- **Technologies**: What's being used
- **Runtime Status**: Can the app build and run? (NEW)
- **Environment**: What's needed to run this project (NEW)
- **Blockers**: Issues preventing the app from working (NEW)
- **Assumptions**: What I think about the project's goals
- **Questions**: What needs clarification

**IMPORTANT**: Wait for human confirmation of this assessment before proceeding.

## Output File:

Create `initial-assessment.md` in the project root with your analysis.

## Next Steps:

After human confirms the assessment, proceed to read `workflow.md`.
