# Cursor Rules Collection

> ⚠️ **Important**: If you're using Cursor without rules, you're doing it wrong!

---

This repository contains a collection of custom rules for the [Cursor](https://cursor.sh/) AI coding assistant that significantly enhance its capabilities. These rules provide structure, automation, and consistency to your AI-assisted coding workflow.

## The Future of Development is Here

AI is transforming software development, and Cursor represents a significant leap forward in this evolution. This repository showcases a fundamental paradigm shift in how we build software:

**From:** Developers manually writing every line of code  
**To:** Developers creating rules and specifications that guide AI assistants to generate implementation

This approach fundamentally changes the developer's role from manual coding to:
1. Defining clear specifications for what should be built
2. Establishing technical rules for how code should be written
3. Supervising the AI as it implements solutions
4. Reviewing and refining the output

Cursor, with properly configured rules, is the first practical implementation of this new development model. The rules in this repository aren't just for code formatting or style, they establish a complete development workflow that manages everything from specifications to tasks, knowledge capture, and code commits.

By adopting this rules-based approach, development teams can dramatically accelerate productivity while maintaining quality control. The journey toward AI-augmented development is already here. **And the best part? You can already begin this journey with Cursor today!**

## What are Cursor Rules?

Cursor rules (in .mdc format) are instructions that guide how the AI assistant behaves, processes information, and generates code. They act as a "stdlib" or framework for the AI, ensuring that it follows best practices, coding standards, and project-specific requirements.

Rules allow you to:
- Automate repetitive tasks
- Enforce coding standards
- Implement workflows that boost productivity
- Create specifications that drive implementation
- Maintain consistency across your codebase

## Rules in this Repository

### On-Load Rule
`on-load-rule.mdc`: Establishes critical development principles that must be followed for all development activities.
- Enforces "specifications first" principle - no implementation without specs
- Ensures proper task tracking for all development activities
- Mandates quality assurance with tests for all implementations
- Requires knowledge capture of important learnings
- Acts as the foundation for all other rules in the system

### Specification Management Rule
`specification-management-rule.mdc`: Comprehensive system for creating, validating, and tracking requirements.
- Automatically creates specifications when implementation is requested
- Provides structured format for requirements with clear acceptance criteria
- Includes validation mechanisms to ensure specification quality
- Tracks specification completion status throughout development
- Maintains a complete index of all project specifications

### Development Workflow Rule
`development-workflow-rule.mdc`: Comprehensive development lifecycle system for task tracking, testing, and version control.
- Creates and manages tasks with unique IDs and structured metadata
- Maintains a central task index with status tracking
- Integrates testing frameworks appropriate to the project type
- Handles version control with conventional commit formatting
- Ensures quality assurance through automated testing
- Prevents completion of tasks that don't pass testing
- Automatically validates and updates README to keep documentation in sync with code

### Knowledge Management Rule
`knowledge-management-rule.mdc`: System for capturing, organizing, and applying project knowledge.
- Documents important learnings during implementation
- Organizes and categorizes knowledge for easy retrieval
- Processes and indexes documentation provided by users
- Refines knowledge to extract patterns and insights
- Applies captured knowledge to new development tasks
- Creates cross-references between related information assets

### Project Onboarding Rule
`project-onboarding-rule.mdc`: Automatically analyzes and onboards existing projects into the AI-driven workflow.
- Creates the required directory structure for AI-driven development
- Analyzes existing codebase structure and components
- Discovers and catalogs existing documentation
- Extracts specifications from existing code
- Sets up initial knowledge base and task tracking
- Provides integration options from full onboarding to basic setup

### Command Rules
`command-rules.mdc`: Defines custom commands for AI-assisted development workflows.
- Provides specialized commands for specifications, code, tasks, and more
- Generates visual dashboards of specifications
- Performs code analysis and refactoring recommendations
- Creates project evaluation and progress reports
- Generates detailed code reviews and PR templates
- Produces comprehensive task summaries

### Visualization Rule
`visualization-rule.mdc`: Creates visual representations of project elements.
- Generates specification dependency diagrams and progress visualizations
- Creates task timelines and status visualizations
- Produces knowledge maps and category charts
- Generates system architecture diagrams
- Automatically includes visualizations in reports

### Location Rule
`location-rule.mdc`: Defines standards for organizing rule files in the repository.
- Establishes consistent locations for rule files
- Ensures proper organization of generated files
- Facilitates discovery and maintenance of rules

## Critical Development Principles

All development with these rules follows these non-negotiable principles:

1. **Specifications First**
   - No implementation without proper specifications
   - All user requests for new features trigger specification creation first
   - Specifications stored in structured format with proper indexing

2. **Task Tracking**
   - All development activities tracked as formal tasks
   - Tasks follow proper state transitions: Open → Active → Done
   - Implementation requires formal task completion

3. **Quality Assurance**
   - All code must have corresponding tests where applicable
   - No implementation considered complete without passing tests
   - Code follows project-specific style guidelines

4. **Knowledge Capture**
   - Important learnings documented during implementation
   - Solutions to complex problems captured for future reference
   - Knowledge organized and made discoverable for future use

5. **Documentation Currency**
   - README and documentation kept in sync with implementation
   - Documentation updated after significant code changes
   - API documentation reflects current implementation

## Integrated Workflow

These rules work together to create a seamless development experience:

1. **Starting a Project**
   - Create or onboard a project with `onboard project` or `setup rules`
   - Analyze existing codebase with `analyze existing` if needed
   - Required directory structure is automatically created

2. **Planning and Specifications**
   - Describe feature requirements to the AI
   - Specifications automatically created in `.cursor/specs/`
   - Specifications indexed in `.cursor/SPECS.md`

3. **Task Management**
   - Tasks automatically created from implementation requests
   - Tasks tracked with unique IDs in `.cursor/TASKS.md`
   - Tasks linked to relevant specifications

4. **Implementation and Testing**
   - AI implements code based on specifications
   - Tests automatically created for new implementations
   - Task progress tracked throughout development

5. **Knowledge Management**
   - Important insights captured as learnings
   - Documents organized and indexed for reference
   - Knowledge applied to future development tasks

6. **Version Control**
   - Changes automatically committed after passing tests
   - Commit messages follow conventional format
   - Code quality maintained through pre-commit testing

7. **Documentation Management**
   - README automatically checked after test success
   - Documentation updated to reflect implemented features
   - API reference kept current with implementation

## Getting Started

1. Clone this repository or download the rules
2. Place the .mdc files in your project's `.cursor/rules/` directory
3. Start Cursor and begin interacting with the AI
4. The rules will automatically take effect during your conversations

For new projects, simply run:
```
onboard project
```

For existing projects that need analysis:
```
analyze existing
```

For just setting up the rules without analysis:
```
setup rules
```

## Practical Workflow

Follow this concrete workflow to get the most out of these rules:

1. **Initial Requirements Discussion**
   - Open Cursor and describe your project/feature requirements to the AI
   - The AI will automatically create specification files in `.cursor/specs/` based on your discussion
   - A central `SPECS.md` file will be generated or updated with links to all domain-specific specs

2. **Automatic Task Planning and Management**
   - Cursor AI automatically creates tasks based on your implementation requests
   - Each task receives a unique ID (e.g., TASK-2023-10-15-01) and is tracked in `.cursor/TASKS.md`
   - Tasks are automatically linked to their relevant specifications and include default acceptance criteria
   - The AI manages multiple tasks concurrently, allowing for efficient development planning

3. **Review & Refine Specifications**
   - Review the generated specs files to ensure they accurately capture requirements
   - Continue the conversation with AI to refine specs as needed
   - Each refinement will update the relevant specification files
   - Cursor AI automatically updates task details when specifications change

4. **AI-Driven Development Based on Specifications**
   - Cursor AI activates tasks when implementation begins
   - Simply ask: "Please implement the feature described in specs/auth/login.md"
   - The AI references the specs during implementation and tracks progress against the task
   - If you request a feature without specifications, the AI creates them first before implementation

5. **Automatic Knowledge Capture During Development**
   - Cursor AI identifies and records important insights during development as learnings
   - The AI documents significant discoveries, patterns, and solutions in `.cursor/learnings/`
   - Share reference documents with the AI by placing them in `.cursor/docs/`
   - All knowledge is automatically indexed in `.cursor/LEARNINGS.md` and `.cursor/DOCUMENTS.md` for future reference

6. **Automatic Documentation Updates**
   - After successful tests, Cursor AI checks if README needs updating
   - Documentation is kept in sync with implementation
   - You can explicitly check README currency with `readme check` command
   - Updates are suggested based on implemented but undocumented features

7. **Automatic Commits**
   - As the AI makes changes to files, the git-commit-rule automatically stages and commits them
   - Commits follow conventional commit format (feat, fix, docs, etc.) based on the nature of the change
   - Commit messages are automatically generated with appropriate type, scope, and description
   - Code is only committed after all tests pass

8. **AI-Managed Task Completion and Knowledge Preservation**
   - When implementation is complete and tests pass, Cursor AI marks the task as done
   - The system updates task status, marks specs as completed, and extracts learnings
   - Learnings are preserved in `.cursor/learnings/` with references to relevant files and tasks
   - The task's status is updated in `.cursor/TASKS.md`

9. **Continuous Development Loop**
   - For new features: discuss requirements → AI generates specs → AI creates & manages tasks → AI implements → AI captures knowledge → AI updates documentation → automatic commits
   - For refinements: discuss changes → AI updates specs → AI updates tasks → AI implements changes → AI updates knowledge → AI updates documentation → automatic commits

This workflow ensures all development is specification-driven, task-organized, properly documented, and automatically committed with appropriate metadata. The integrated approach means nothing gets lost - requirements, implementation details, insights, and documentation are all preserved and linked together. You simply guide the process through conversation while Cursor AI handles the entire workflow.

## Inspiration

This approach was inspired by [Geoffrey Huntley's method](https://ghuntley.com/specs/) of using Cursor AI effectively. Huntley demonstrates how combining specifications with technical rules creates a powerful workflow that can dramatically increase development productivity.

As Huntley explains:
> "When you use '/specs' method with the 'stdlib' method in conjunction with a programming language that provides compiler soundness (driven by good types) and compiler errors, the results are incredible. You can drive hands-free output of N factor (entire weeks' worth) of co-workers in hours."

## Future Enhancements

### Automatic README Updates

A promising enhancement being added to this system is a rule that automatically checks and updates the project's README file:
- After successful unit testing
- Before commits
- When significant changes are made to the codebase

This ensures documentation stays in sync with implementation, providing:
- Up-to-date project information
- Current installation instructions
- Latest feature descriptions
- Accurate API documentation

This feature reduces the manual overhead of maintaining documentation while ensuring it accurately reflects the current state of the project.

## Something Missing?

One of the most powerful aspects of Cursor is its ability to extend itself! You can ask Cursor to create new rules that address your specific workflow needs:

### How to Ask Cursor to Implement New Rules

1. **Identify a Workflow Pain Point**: Think about a repetitive task or pattern you'd like to automate

2. **Ask Cursor to Create a Rule**: Use prompts like:
   ```
   Create a Cursor IDE MDC rule that automatically [describes desired behavior].
   The rule should be saved to .cursor/rules/[rule-name].mdc
   ```

3. **Example Prompts**:
   - "Create a Cursor IDE MDC rule that automatically generates unit tests whenever I create a new function"
   - "Create a Cursor MDC rule for TypeScript files that enforces consistent error handling patterns"
   - "Create a rule that inserts license headers into new files based on file type"

4. **Refine the Rule**: Cursor will generate a rule file, but you can continue the conversation to refine it:
   ```
   That looks good, but can you modify the rule to also handle [additional case]?
   ```

5. **Test and Iterate**: Apply the rule in your workflow and ask Cursor to make adjustments as needed

This meta-capability - using Cursor to extend Cursor - demonstrates the true power of rule-based AI assistance. You're not limited to the rules in this repository; you can create a completely customized workflow tailored to your project's needs.

## Contributing

Feel free to contribute your own rules or improvements to existing ones via pull requests.

## License

MIT License

Copyright (c) 2023 

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

"If you want to build a ship, don't drum up people to collect wood and don't assign them tasks and work, but rather teach them to long for the endless immensity of the sea." - Antoine de Saint-Exupéry

_In the same way, effective AI systems don't just execute code, but operate within a framework of principles and specifications that guide them toward building solutions that fulfill the true vision of what we seek to create._
