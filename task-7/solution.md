# Task 7 Solution: SPECKit Plus Concepts

## 1. What is SPECKit Plus?
SPECKit Plus is a comprehensive framework designed to implement the **SDD-RI (Specification-Driven Development with Recursive Intelligence)** methodology. It provides a structured, AI-native approach to software development that emphasizes "Horizontal/Vertical Intelligence" and a "two-output philosophy" (producing both code and verification/documentation). It guides developers through a disciplined lifecycle—from defining global quality standards to executing atomic tasks—ensuring that AI is used as a collaborative partner rather than just an autonomous generator.

## 2. Core Concepts

### 1️⃣ /constitution
The **Constitution** defines the immutable, project-wide quality standards that apply to *all* work within a project. Unlike specifications which are feature-specific, the Constitution sets global rules such as citation styles, coding standards, plagiarism limits, and security protocols. It acts as the first quality gate, ensuring that every subsequent phase (specification, plan, tasks) adheres to these foundational principles.

### 2️⃣ /specify
The **Specify** phase is where vague ideas are translated into crystal-clear, objective requirements. It focuses on defining "what success looks like" through business and user-centric criteria rather than just technical checks. This phase involves a pre-specification conversation to clarify intent and uses the SMART test to ensure requirements are Specific, Measurable, Achievable, Relevant, and Time-bound. A clear specification is the prerequisite for any effective AI implementation.

### 3️⃣ /plan
The **Plan** phase transforms the "What" (specification) into the "How" (architecture and implementation strategy). It involves analyzing the specification to break it down into components, order dependencies, and identify necessary design decisions. This phase also includes creating **ADRs (Architectural Decision Records)** to document key technical choices. The goal is to create a detailed roadmap that guides the execution, ensuring that the architecture supports the specification's success criteria.

### 4️⃣ /tasks
The **Tasks** phase breaks the implementation plan into atomic, manageable units of work, typically taking 15-30 minutes each. Each task must have a single, clear acceptance criterion and produce a verifiable output. This phase introduces the **Checkpoint Pattern**, which establishes critical boundaries where human review is required. By structuring work into small, verifiable steps, it prevents AI from drifting off course and ensures steady, measurable progress.

### 5️⃣ /implement
The **Implement** phase is the execution stage where the defined tasks are carried out. In SDD-RI, implementation is not about letting AI work autonomously in a black box; it is a collaborative process. The developer uses the `/sp.implement` command to orchestrate the AI, reviewing outputs against the specification at each checkpoint. The focus is on validating that the work meets the pre-defined success criteria, ensuring high-quality, spec-compliant results.
