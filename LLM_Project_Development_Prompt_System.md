# LLM Project Development Prompt System

_A systematic approach to specification, planning, and execution of development projects using LLM assistance_

## Table of Contents

1. [Overview](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#overview)
2. [Prompt Phases](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#prompt-phases)
3. [Project Specification Templates](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#project-specification-templates)
4. [Confirmation Protocols](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#confirmation-protocols)
5. [Planning & Chunking Strategies](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#planning--chunking-strategies)
6. [Git Project Phases](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#git-project-phases)
7. [Phase Execution Templates](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#phase-execution-templates)
8. [Quality Gates](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#quality-gates)
9. [Example Project Walkthrough](https://claude.ai/chat/875a2df9-f007-4a35-9ac3-b3f68689a057#example-project-walkthrough)

***

## Overview

This system provides structured prompts and workflows for collaborating with LLMs on development projects. It ensures comprehensive specification, proper planning, and systematic execution while maintaining quality and security standards.

### Core Principles

* **Explicit Requirements Capture**: Every detail specified upfront
* **Confirmation Before Action**: No assumptions, explicit validation
* **Phased Delivery**: Break complex projects into manageable chunks
* **Quality Gates**: Validation at each phase transition
* **Git-First Approach**: Version control integrated from the start

***

## Prompt Phases

### Phase 1: SPECIFICATION

**Objective**: Capture complete project requirements with no ambiguity

### Phase 2: CONFIRMATION

**Objective**: Validate understanding and get explicit approval

### Phase 3: PLANNING

**Objective**: Break down into phases with clear deliverable

### Phase 4: CHUNKING

**Objective**: Define granular tasks within each phase

### Phase 5: EXECUTION

**Objective**: Implement with continuous validation

### Phase 6: VALIDATION

**Objective**: Test, review, and approve each deliverable

***

## Project Specification Templates

### 🎯 SPECIFICATION PROMPT TEMPLATE

```
# PROJECT SPECIFICATION PHASE

I need to build a [PROJECT_TYPE] project. Before we proceed with any planning or implementation, I need you to help me capture ALL requirements comprehensively.

## CRITICAL: SPECIFICATION REQUIREMENTS
Please ask me detailed questions about EACH of the following areas. Do NOT proceed to planning until I have provided complete answers to ALL areas:

### 1. FUNCTIONAL REQUIREMENTS
- What specific features and capabilities must the system provide?
- What are the user workflows and use cases?
- What business logic and rules must be implemented?
- What integrations with external systems are required?

### 2. TECHNICAL REQUIREMENTS
- Target platform/environment (web, mobile, desktop, server)?
- Technology stack preferences or constraints?
- Performance requirements (users, transactions, response times)?
- Security requirements and compliance needs?
- Database requirements and data models?

### 3. PROJECT CONSTRAINTS
- Timeline and deadline requirements?
- Budget or resource constraints?
- Team size and skill levels?
- Deployment environment and infrastructure?

### 4. QUALITY REQUIREMENTS
- Testing requirements (unit, integration, e2e)?
- Documentation standards needed?
- Code quality and coverage expectations?
- Monitoring and logging requirements?

### 5. DELIVERY REQUIREMENTS
- How should the project be delivered (phases, MVP, etc.)?
- What are the acceptance criteria for completion?
- Who are the stakeholders requiring approval?
- What is the deployment and go-live process?

## INSTRUCTION
Ask me focused questions about each area above. Wait for my complete answers before moving to the next area. Once ALL areas are fully specified, confirm you have everything needed and ask for explicit approval to proceed to planning.

CONFIRM YOU UNDERSTAND THIS SPECIFICATION PHASE REQUIREMENT.
```

### 🔍 DETAILED REQUIREMENTS CAPTURE

```
# REQUIREMENTS DEEP DIVE

For the [SPECIFIC_AREA] you mentioned, I need more detailed information:

## CURRENT AREA: [FUNCTIONAL/TECHNICAL/CONSTRAINTS/QUALITY/DELIVERY]

### SPECIFIC QUESTIONS:
1. [DETAILED_QUESTION_1]
2. [DETAILED_QUESTION_2]
3. [DETAILED_QUESTION_3]

### EXAMPLES FOR CLARITY:
- Example scenario: [SPECIFIC_EXAMPLE]
- Expected behavior: [EXPECTED_OUTCOME]
- Edge case consideration: [EDGE_CASE]

### VALIDATION CHECKLIST:
Please confirm each of the following:
- [ ] [REQUIREMENT_1] is correct as specified
- [ ] [REQUIREMENT_2] includes all necessary details
- [ ] [REQUIREMENT_3] covers all edge cases

## NEXT STEPS
Once you provide complete answers above, I will:
1. Summarize your requirements for this area
2. Ask for your confirmation that the summary is accurate
3. Move to the next requirements area

PLEASE PROVIDE DETAILED ANSWERS TO ALL QUESTIONS ABOVE.
```

***

## Confirmation Protocols

### ✅ CONFIRMATION PROMPT TEMPLATE

```
# PROJECT SPECIFICATION CONFIRMATION

Based on our discussion, here is my complete understanding of your project requirements:

## PROJECT SUMMARY
**Project Type**: [PROJECT_TYPE]
**Primary Objective**: [MAIN_GOAL]
**Target Users**: [USER_GROUPS]

## FUNCTIONAL REQUIREMENTS
### Core Features:
1. [FEATURE_1] - [DETAILED_DESCRIPTION]
2. [FEATURE_2] - [DETAILED_DESCRIPTION]
3. [FEATURE_3] - [DETAILED_DESCRIPTION]

### User Workflows:
1. [WORKFLOW_1]: [STEP_BY_STEP_PROCESS]
2. [WORKFLOW_2]: [STEP_BY_STEP_PROCESS]

### Business Rules:
- [RULE_1]: [SPECIFIC_IMPLEMENTATION]
- [RULE_2]: [SPECIFIC_IMPLEMENTATION]

### External Integrations:
- [INTEGRATION_1]: [PURPOSE_AND_SCOPE]
- [INTEGRATION_2]: [PURPOSE_AND_SCOPE]

## TECHNICAL REQUIREMENTS
**Technology Stack**: [SPECIFIC_TECHNOLOGIES]
**Platform**: [TARGET_PLATFORM]
**Database**: [DATABASE_CHOICE_AND_REQUIREMENTS]
**Performance**: [SPECIFIC_METRICS]
**Security**: [SECURITY_REQUIREMENTS]

## PROJECT CONSTRAINTS
**Timeline**: [SPECIFIC_DEADLINES]
**Resources**: [TEAM_AND_BUDGET]
**Infrastructure**: [DEPLOYMENT_REQUIREMENTS]

## QUALITY REQUIREMENTS
**Testing**: [TESTING_STRATEGY]
**Documentation**: [DOCUMENTATION_REQUIREMENTS]
**Monitoring**: [MONITORING_STRATEGY]

## DELIVERY APPROACH
**Delivery Method**: [PHASED/MVP/BIG_BANG]
**Acceptance Criteria**: [SPECIFIC_CRITERIA]
**Stakeholders**: [APPROVAL_REQUIRED_FROM]

## CRITICAL CONFIRMATION REQUIRED
Please review the above specification carefully and confirm:

1. **ACCURACY CHECK**: Is every detail above correct as you intended?
2. **COMPLETENESS CHECK**: Are there any missing requirements or details?
3. **PRIORITY CHECK**: Are the priorities and importance levels correct?
4. **CONSTRAINT CHECK**: Are all constraints and limitations captured?

Please respond with:
- "CONFIRMED - Proceed to planning" if everything is accurate and complete
- "CHANGES REQUIRED" followed by specific corrections needed

DO NOT PROCEED TO PLANNING UNTIL YOU RECEIVE EXPLICIT CONFIRMATION.
```

***

## Planning & Chunking Strategies

### 📋 PLANNING PROMPT TEMPLATE

```
# PROJECT PLANNING PHASE

Now that requirements are confirmed, I will create a comprehensive project plan.

## PLANNING APPROACH
I will break this project into logical phases with:
- Clear deliverables for each phase
- Dependencies between phases identified
- Risk mitigation strategies
- Quality gates at each phase boundary

## PROPOSED PHASE STRUCTURE

### PHASE 0: PROJECT SETUP & FOUNDATION
**Duration**: [TIME_ESTIMATE]
**Objective**: Establish development environment and project foundation
**Key Deliverables**:
- Git repository setup with branching strategy
- Development environment configuration
- CI/CD pipeline basic setup
- Project structure and standards implementation
- Initial documentation framework

**Definition of Done**:
- [ ] Repository created with proper structure
- [ ] Development environment documented and tested
- [ ] Basic CI/CD pipeline operational
- [ ] Team can clone and run project locally
- [ ] Architecture documentation approved

### PHASE 1: [CORE_FOUNDATION_PHASE]
**Duration**: [TIME_ESTIMATE]
**Objective**: [PHASE_OBJECTIVE]
**Key Deliverables**:
- [DELIVERABLE_1]: [SPECIFIC_OUTCOME]
- [DELIVERABLE_2]: [SPECIFIC_OUTCOME]
- [DELIVERABLE_3]: [SPECIFIC_OUTCOME]

**Dependencies**: [DEPENDENCIES_FROM_PREVIOUS_PHASES]
**Risks**: [IDENTIFIED_RISKS_AND_MITIGATIONS]

**Definition of Done**:
- [ ] [SPECIFIC_CRITERIA_1]
- [ ] [SPECIFIC_CRITERIA_2]
- [ ] [SPECIFIC_CRITERIA_3]
- [ ] Phase deliverables tested and approved
- [ ] Documentation updated

### PHASE 2: [FEATURE_DEVELOPMENT_PHASE]
**Duration**: [TIME_ESTIMATE]
**Objective**: [PHASE_OBJECTIVE]
**Key Deliverables**:
- [DELIVERABLE_1]: [SPECIFIC_OUTCOME]
- [DELIVERABLE_2]: [SPECIFIC_OUTCOME]

**Definition of Done**:
- [ ] [SPECIFIC_CRITERIA_1]
- [ ] [SPECIFIC_CRITERIA_2]
- [ ] All tests passing
- [ ] Security review completed
- [ ] Performance benchmarks met

### PHASE N: [FINAL_PHASE]
**Duration**: [TIME_ESTIMATE]
**Objective**: Production deployment and go-live
**Key Deliverables**:
- Production deployment
- Documentation finalization
- User training materials
- Support procedures

## OVERALL PROJECT TIMELINE
**Total Estimated Duration**: [TOTAL_TIME]
**Key Milestones**:
- [MILESTONE_1]: [DATE]
- [MILESTONE_2]: [DATE]
- [MILESTONE_3]: [DATE]

## PHASE CONFIRMATION REQUIRED
Please review this phase breakdown and confirm:
1. **PHASE LOGIC**: Do the phases make sense and build logically?
2. **DELIVERABLES**: Are the deliverables clear and appropriate?
3. **TIMELINE**: Are the time estimates realistic?
4. **DEPENDENCIES**: Are phase dependencies correctly identified?

Respond with "PLANNING APPROVED" to proceed to detailed task chunking, or request specific changes.
```

### 🧩 CHUNKING PROMPT TEMPLATE

```
# PHASE CHUNKING - DETAILED TASK BREAKDOWN

## TARGET PHASE: [PHASE_NAME]
**Phase Objective**: [OBJECTIVE]
**Estimated Duration**: [DURATION]

I will now break this phase into specific, actionable tasks that can be implemented systematically.

## TASK CHUNKING STRATEGY
Each task will be:
- Small enough to complete in 1-4 hours
- Self-contained with clear inputs/outputs
- Testable independently
- Documented with acceptance criteria

## DETAILED TASK BREAKDOWN

### TASK CATEGORY 1: [CATEGORY_NAME]
**Objective**: [CATEGORY_OBJECTIVE]

#### Task 1.1: [TASK_NAME]
**Description**: [DETAILED_TASK_DESCRIPTION]
**Estimated Time**: [TIME_ESTIMATE]
**Prerequisites**: [DEPENDENCIES]
**Deliverables**:
- [SPECIFIC_OUTPUT_1]
- [SPECIFIC_OUTPUT_2]
**Acceptance Criteria**:
- [ ] [SPECIFIC_CRITERIA_1]
- [ ] [SPECIFIC_CRITERIA_2]
- [ ] [SPECIFIC_CRITERIA_3]
**Test Requirements**:
- [TESTING_APPROACH]
**Git Branch Strategy**: `feature/[TASK-ID]-[TASK-NAME]`

#### Task 1.2: [TASK_NAME]
[SAME_STRUCTURE_AS_ABOVE]

### TASK CATEGORY 2: [CATEGORY_NAME]
[REPEAT_STRUCTURE_FOR_EACH_CATEGORY]

## TASK EXECUTION ORDER
**Sequential Tasks** (must be completed in order):
1. Task 1.1 → Task 1.2 → Task 1.3
2. Task 2.1 → Task 2.3

**Parallel Tasks** (can be worked on simultaneously):
- Task 2.2 can run parallel with Task 1.x series
- Task 3.1 can start after Task 1.1 completes

## TASK VALIDATION CHECKLIST
For each task completion:
- [ ] Code implemented and tested
- [ ] Unit tests written and passing
- [ ] Integration tests passing
- [ ] Code review completed
- [ ] Documentation updated
- [ ] Git branch merged to development
- [ ] Task marked as complete in project tracker

## CHUNKING CONFIRMATION REQUIRED
Please confirm:
1. **TASK GRANULARITY**: Are tasks appropriately sized?
2. **TASK DEPENDENCIES**: Are dependencies correctly identified?
3. **ACCEPTANCE CRITERIA**: Are criteria clear and testable?
4. **EXECUTION ORDER**: Does the task sequence make sense?

Respond with "CHUNKING APPROVED - BEGIN PHASE [X]" to start implementation.
```

***

## Git Project Phases

### 🔀 GIT WORKFLOW SETUP PROMPT

```
# GIT PROJECT STRUCTURE & WORKFLOW

I will establish a comprehensive Git workflow that supports our phased development approach.

## REPOSITORY SETUP

### Initial Repository Structure
```

project-root/ ├── .github/ │ ├── workflows/ # CI/CD workflows │ ├── ISSUE\_TEMPLATE/ # Issue templates │ └── PULL\_REQUEST\_TEMPLATE.md ├── docs/ │ ├── architecture/ # Architecture documents │ ├── api/ # API documentation │ └── deployment/ # Deployment guides ├── src/ # Source code ├── tests/ # Test files ├── scripts/ # Build and deployment scripts ├── .gitignore ├── README.md ├── CONTRIBUTING.md └── CHANGELOG.md

````

### Branch Strategy
**Main Branches**:
- `main` - Production-ready code
- `develop` - Integration branch for features
- `staging` - Pre-production testing

**Feature Branches**:
- `feature/[PHASE-ID]-[TASK-ID]-[TASK-NAME]`
- Example: `feature/phase1-task1.2-user-authentication`

**Support Branches**:
- `hotfix/[ISSUE-ID]-[DESCRIPTION]`
- `release/[VERSION-NUMBER]`

## PHASE-BASED GIT WORKFLOW

### Phase 0: Repository Foundation
```bash
# Repository initialization
git init
git add .
git commit -m "Initial project structure and documentation"

# Branch setup
git checkout -b develop
git checkout -b staging

# Protection rules setup (via GitHub/GitLab interface)
# - main: Require PR, require reviews, require status checks
# - develop: Require PR, require CI to pass
# - staging: Require PR from develop only
````

### Phase Development Workflow

```bash
# Starting a new phase
git checkout develop
git pull origin develop
git checkout -b feature/phase[N]-setup
git push -u origin feature/phase[N]-setup

# For each task in the phase
git checkout develop
git pull origin develop
git checkout -b feature/phase[N]-task[X]-[TASK-NAME]

# Work on task...
git add .
git commit -m "feat(phase[N]): implement [TASK_DESCRIPTION]

- Add [SPECIFIC_CHANGE_1]
- Implement [SPECIFIC_CHANGE_2]
- Test [SPECIFIC_TEST_SCENARIO]

Closes #[TASK_ISSUE_NUMBER]"

# Push and create PR
git push -u origin feature/phase[N]-task[X]-[TASK-NAME]
# Create PR to develop branch
```

### Phase Completion Workflow

```bash
# Phase completion checklist
# 1. All phase tasks completed and merged to develop
# 2. Integration tests passing on develop
# 3. Phase documentation updated
# 4. Phase review completed

# Merge to staging for testing
git checkout staging
git pull origin staging
git merge develop
git push origin staging

# Deploy to staging environment for testing
# Run full test suite
# Stakeholder review and approval

# Merge to main for production
git checkout main
git pull origin main
git merge staging
git tag -a v[VERSION] -m "Release version [VERSION] - Phase [N] completion"
git push origin main --tags
```

## COMMIT MESSAGE STANDARDS

### Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

* `feat`: New feature
* `fix`: Bug fix
* `docs`: Documentation changes
* `style`: Code style changes (formatting, etc.)
* `refactor`: Code refactoring
* `test`: Adding or updating tests
* `chore`: Maintenance tasks

### Examples

```bash
feat(auth): implement JWT authentication

- Add JWT token generation and validation
- Implement login/logout endpoints
- Add middleware for protected routes
- Include token refresh mechanism

Closes #23, #24
```

```bash
fix(database): resolve connection pool exhaustion

- Increase connection pool size to 20
- Add connection timeout configuration
- Implement proper connection cleanup
- Add monitoring for pool status

Fixes #45
```

## GIT PHASE GATES

### Phase Merge Criteria

Before merging any phase to main:

* \[ ] All phase tasks completed
* \[ ] All tests passing (unit, integration, e2e)
* \[ ] Code coverage meets requirements (80%+)
* \[ ] Security scan completed with no critical issues
* \[ ] Performance benchmarks met
* \[ ] Documentation updated
* \[ ] Stakeholder approval received

### Automated Checks (CI/CD)

```yaml
# .github/workflows/phase-gate.yml
name: Phase Gate Checks

on:
  pull_request:
    branches: [ main, staging ]

jobs:
  quality-gate:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v4
    
    - name: Run Tests
      run: npm test
      
    - name: Check Coverage
      run: npm run test:coverage
      
    - name: Security Scan
      run: npm audit
      
    - name: Performance Test
      run: npm run test:performance
      
    - name: Documentation Check
      run: npm run docs:validate
```

## GIT WORKFLOW CONFIRMATION

Please confirm this Git workflow setup:

1. **BRANCH STRATEGY**: Does the branching model work for your team?
2. **PHASE INTEGRATION**: Does the phase-based workflow align with project needs?
3. **QUALITY GATES**: Are the merge criteria appropriate?
4. **COMMIT STANDARDS**: Are the commit message standards clear?

Respond with "GIT WORKFLOW APPROVED" to proceed with repository setup.

```

---

## Phase Execution Templates

### 🚀 PHASE EXECUTION PROMPT
```

# PHASE EXECUTION - \[PHASE\_NAME]

We are now beginning execution of Phase \[N]: \[PHASE\_NAME]

## PHASE CONTEXT

**Objective**: \[PHASE\_OBJECTIVE] **Duration**: \[ESTIMATED\_DURATION] **Key Deliverables**: \[MAIN\_DELIVERABLES]

## PRE-EXECUTION CHECKLIST

Before starting any implementation, confirm:

* \[ ] Previous phase completely finished and approved
* \[ ] Development environment ready and tested
* \[ ] All prerequisites and dependencies available
* \[ ] Git branch created for this phase
* \[ ] Project tracker updated with phase tasks
* \[ ] Team members assigned to tasks

## TASK EXECUTION APPROACH

### Current Task: \[TASK\_ID] - \[TASK\_NAME]

**Objective**: \[TASK\_OBJECTIVE] **Estimated Time**: \[TIME\_ESTIMATE]

**IMPLEMENTATION PROTOCOL**:

1. **BEFORE CODING**:

   * Review task requirements and acceptance criteria
   * Confirm understanding of inputs and expected outputs
   * Identify any clarifications needed
   * Plan implementation approach

2. **DURING IMPLEMENTATION**:

   * Follow coding standards from development pack
   * Write tests as you implement (TDD approach)
   * Commit frequently with descriptive messages
   * Document any deviations or decisions

3. **AFTER IMPLEMENTATION**:

   * Run all tests and ensure they pass
   * Update documentation
   * Create pull request with proper description
   * Request code review

## TASK VALIDATION CHECKLIST

For each completed task, verify:

* \[ ] **FUNCTIONALITY**: Does it work as specified?
* \[ ] **TESTING**: Are tests written and passing?
* \[ ] **SECURITY**: Security requirements met?
* \[ ] **PERFORMANCE**: Meets performance criteria?
* \[ ] **DOCUMENTATION**: Code and API documented?
* \[ ] **STANDARDS**: Follows coding standards?
* \[ ] **INTEGRATION**: Works with existing code?

## CONTINUOUS VALIDATION

During phase execution:

* Daily progress updates required
* Blockers identified and escalated immediately
* Regular integration testing on develop branch
* Documentation kept current with implementation

## READY TO BEGIN?

Confirm readiness to start implementation:

* \[ ] Phase setup complete
* \[ ] First task clearly understood
* \[ ] Development environment ready
* \[ ] Quality standards clear

Respond with "READY TO IMPLEMENT TASK \[TASK\_ID]" to begin coding.

```

### 🔍 TASK IMPLEMENTATION PROMPT
```

# TASK IMPLEMENTATION - \[TASK\_ID]

## TASK CONTEXT

**Task**: \[TASK\_NAME] **Description**: \[DETAILED\_DESCRIPTION] **Acceptance Criteria**: \[CRITERIA\_LIST]

## IMPLEMENTATION REQUEST

I need you to implement this task following these requirements:

### TECHNICAL REQUIREMENTS

* **Technology Stack**: \[SPECIFIED\_STACK]
* **Coding Standards**: Follow development standards pack
* **Security Requirements**: \[SPECIFIC\_SECURITY\_NEEDS]
* **Performance Requirements**: \[PERFORMANCE\_CRITERIA]

### IMPLEMENTATION STRUCTURE

Please provide:

1. **FILE STRUCTURE**: Show me the files that will be created/modified
2. **IMPLEMENTATION PLAN**: Step-by-step approach
3. **TEST STRATEGY**: How this will be tested
4. **INTEGRATION POINTS**: How this connects to existing code

### CODE REQUIREMENTS

* Include comprehensive error handling
* Add appropriate logging
* Follow security best practices
* Include input validation
* Add proper documentation/comments

### DELIVERABLE FORMAT

Provide the implementation in this format:

1. **Implementation Overview**
2. **File Structure and Changes**
3. **Complete Code Implementation**
4. **Test Code**
5. **Documentation Updates**
6. **Integration Instructions**

## CRITICAL: BEFORE IMPLEMENTING

Please confirm your understanding by describing:

1. What this task will accomplish
2. How it fits into the overall system
3. What the main technical challenges are
4. How you will test it

Wait for my confirmation before providing the implementation.

```

---

## Quality Gates

### ✅ QUALITY GATE PROMPT TEMPLATE
```

# QUALITY GATE CHECKPOINT - \[PHASE/TASK]

Before proceeding to the next phase/task, we must validate that all quality requirements are met.

## QUALITY GATE CRITERIA

### FUNCTIONAL VALIDATION

* \[ ] **Requirements Met**: All specified requirements implemented
* \[ ] **Acceptance Criteria**: All criteria satisfied and tested
* \[ ] **User Stories**: All user stories completed and validated
* \[ ] **Edge Cases**: Edge cases identified and handled

### TECHNICAL VALIDATION

* \[ ] **Code Quality**: Follows coding standards and best practices
* \[ ] **Test Coverage**: Minimum 80% code coverage achieved
* \[ ] **Performance**: Meets performance benchmarks
* \[ ] **Security**: Security requirements implemented and tested
* \[ ] **Documentation**: Code and API documentation complete

### INTEGRATION VALIDATION

* \[ ] **Unit Tests**: All unit tests passing
* \[ ] **Integration Tests**: Integration tests passing
* \[ ] **System Tests**: End-to-end tests passing
* \[ ] **Regression Tests**: No regressions introduced

### OPERATIONAL VALIDATION

* \[ ] **Deployment**: Can be deployed to target environment
* \[ ] **Monitoring**: Monitoring and logging implemented
* \[ ] **Backup**: Backup procedures tested
* \[ ] **Recovery**: Recovery procedures validated

## QUALITY GATE ASSESSMENT

Please provide evidence for each criterion:

### FUNCTIONAL EVIDENCE

* Screenshots or recordings of working features
* Test execution reports
* User acceptance test results

### TECHNICAL EVIDENCE

* Code review results
* Test coverage reports
* Performance test results
* Security scan results

### INTEGRATION EVIDENCE

* CI/CD pipeline results
* Integration test reports
* System test results

### OPERATIONAL EVIDENCE

* Deployment verification
* Monitoring dashboard screenshots
* Backup/recovery test results

## GATE DECISION

Based on the evidence provided:

**GATE STATUS**: \[PASS/FAIL/CONDITIONAL]

**JUSTIFICATION**: \[DETAILED\_REASONING]

**ACTION REQUIRED**:

* If PASS: Proceed to next phase
* If CONDITIONAL: Address specific issues before proceeding
* If FAIL: Return to implementation phase

**SPECIFIC ACTIONS** (if not PASS):

1. \[SPECIFIC\_ACTION\_1]
2. \[SPECIFIC\_ACTION\_2]
3. \[SPECIFIC\_ACTION\_3]

## GATE CONFIRMATION REQUIRED

Stakeholder approval required before proceeding:

* \[ ] Technical lead approval
* \[ ] Project manager approval
* \[ ] Quality assurance approval
* \[ ] Security team approval (if applicable)

Respond with "QUALITY GATE PASSED - PROCEED" or "QUALITY GATE FAILED - REMEDIATE" with specific actions.

```

---

## Example Project Walkthrough

### 📖 COMPLETE PROJECT EXAMPLE
```

# EXAMPLE: E-COMMERCE API PROJECT WALKTHROUGH

This example demonstrates the complete prompt system workflow for building an e-commerce API.

## PHASE 1: SPECIFICATION

### Initial Specification Prompt

"I need to build an e-commerce API project. Before we proceed with any planning or implementation, I need you to help me capture ALL requirements comprehensively.

\[Use the SPECIFICATION PROMPT TEMPLATE above]"

### Requirements Captured

* **Functional**: Product catalog, shopping cart, user management, order processing, payment integration
* **Technical**: REST API, Node.js/Express, PostgreSQL, JWT authentication, Stripe payments
* **Constraints**: 3-month timeline, 2 developers, AWS deployment
* **Quality**: 80% test coverage, API documentation, performance <200ms response
* **Delivery**: MVP in 6 weeks, full feature set in 12 weeks

## PHASE 2: CONFIRMATION

### Confirmation Summary

\[Detailed summary using CONFIRMATION PROMPT TEMPLATE]

**Result**: "CONFIRMED - Proceed to planning"

## PHASE 3: PLANNING

### Phase Breakdown

* **Phase 0**: Project setup (1 week)
* **Phase 1**: User management and authentication (2 weeks)
* **Phase 2**: Product catalog API (2 weeks)
* **Phase 3**: Shopping cart functionality (1.5 weeks)
* **Phase 4**: Order processing (2 weeks)
* **Phase 5**: Payment integration (1.5 weeks)
* **Phase 6**: Testing and deployment (2 weeks)

**Result**: "PLANNING APPROVED"

## PHASE 4: CHUNKING (Example - Phase 1)

### Phase 1 Task Breakdown

* **Task 1.1**: User registration endpoint (4 hours)
* **Task 1.2**: User login with JWT (3 hours)
* **Task 1.3**: Password reset functionality (4 hours)
* **Task 1.4**: User profile management (3 hours)
* **Task 1.5**: Authentication middleware (2 hours)

**Result**: "CHUNKING APPROVED - BEGIN PHASE 1"

## PHASE 5: EXECUTION (Example - Task 1.1)

### Task 1.1 Implementation Request

```
# TASK IMPLEMENTATION - 1.1

## TASK CONTEXT
**Task**: User registration endpoint
**Description**: Create POST /api/users/register endpoint that accepts user data, validates it, hashes password, and stores in database
**Acceptance Criteria**: 
- Accepts email, password, firstName, lastName
- Validates email format and password strength
- Returns 400 for invalid data, 409 for existing email, 201 for success
- Password hashed using bcrypt
- Returns JWT token on successful registration

[Continue with full implementation request...]
```

## PHASE 6: VALIDATION

### Quality Gate Results

* **Functional**: ✅ All endpoints working as specified
* **Technical**: ✅ 85% test coverage, performance under 150ms
* **Integration**: ✅ All tests passing
* **Operational**: ✅ Deployed to staging successfully

**Result**: "QUALITY GATE PASSED - PROCEED TO PHASE 2"

## PROJECT COMPLETION

### Final Deliverables

* Complete e-commerce API with 15 endpoints
* 87% test coverage
* Comprehensive API documentation
* Deployed to AWS with CI/CD pipeline
* Performance averaging 120ms response time
* Security scan passed with no critical issues

**Project Status**: SUCCESSFULLY COMPLETED ON TIME

```

---

## Best Practices Summary

### 🎯 KEY SUCCESS FACTORS

1. **Never Skip Specification**: Always capture complete requirements before planning
2. **Explicit Confirmation**: Get written approval at each phase gate
3. **Small Task Chunks**: Keep tasks to 1-4 hours for manageable implementation
4. **Continuous Validation**: Test and validate continuously, not just at the end
5. **Git Discipline**: Use branching strategy consistently for all changes
6. **Documentation First**: Update documentation as you implement, not after
7. **Quality Gates**: Never compromise on quality criteria
8. **Stakeholder Engagement**: Keep stakeholders informed and engaged throughout

### 🚨 COMMON PITFALLS TO AVOID

- Starting implementation before complete specification
- Assuming understanding without explicit confirmation
- Making phases too large (>2 weeks)
- Skipping testing until the end
- Poor Git hygiene and branching
- Outdated or missing documentation
- Bypassing quality gates due to time pressure
- Lack of stakeholder communication

### 📋 PROMPT CHECKLIST

Before using any prompt in this system:
- [ ] Context is clearly established
- [ ] Requirements for response are explicit
- [ ] Confirmation mechanism is defined
- [ ] Next steps are clearly outlined
- [ ] Quality criteria are specified
- [ ] Success/failure conditions are clear

---

*This prompt system ensures systematic, high-quality development projects with clear deliverables, proper validation, and comprehensive documentation throughout the entire development lifecycle.*
```
