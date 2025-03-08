# Prompt Engineering Patterns

This document catalogs successful patterns for prompt engineering discovered through our collaborative projects. These patterns represent reusable approaches that have proven effective in facilitating productive human-AI collaboration.

## Foundational Patterns

### Clear Goal, Open Implementation

**Pattern:** Define what needs to be accomplished while leaving room for the AI to suggest implementation approaches.

**Example:**

"I need a way to exchange drawings between humans and AI in a chat interface. The current approach using base64 images is too bulky and error-prone."

Instead of:

"Create a vector-based drawing exchange format with these specific data structures..."

**Why it works:** This pattern leverages the AI's ability to explore multiple solution spaces while keeping the collaboration focused on a clear objective. It allows for unexpected approaches that the human might not have considered.

### Progressive Refinement

**Pattern:** Start with basic functionality, then iteratively enhance specific aspects.

**Example:**

"Let's create a minimal drawing application first, then refine it to handle errors better and add more features."

Followed later by:

"Now that the basic functionality works, can we refactor it to be more modular and educational?"

**Why it works:** This creates a successful feedback loop where each iteration builds on demonstrated success rather than trying to perfect everything at once. It also allows for course correction based on what's learned during implementation.

### Explicit Learning Objectives

**Pattern:** Clearly state what you want to learn or understand through the process.

**Example:**

"Please focus on learnability over optimization. I want to study what you've created."

**Why it works:** This guides the AI to prioritize explanatory content and educational value in its responses, resulting in code and documentation that serves as a learning resource, not just a functional solution.

## Collaborative Problem-Solving Patterns

### Descriptive Error Reporting

**Pattern:** Report errors with context and details rather than just stating something doesn't work.

**Example:**

"I'm getting this error message: 'Error: Failed to execute 'writeText' on 'Clipboard'. Can you explain what's happening and suggest alternatives?"

**Why it works:** This gives the AI specific information to diagnose the problem and understand the context, leading to more targeted and effective solutions.

### Collaborative Decision Points

**Pattern:** Explicitly mark key decision points and discuss options before implementation.

**Example:**

**Why it works:** This gives the AI specific information to diagnose the problem and understand the context, leading to more targeted and effective solutions.

### Collaborative Decision Points

**Pattern:** Explicitly mark key decision points and discuss options before implementation.

**Example:**

"We're facing an issue with large base64 strings. What approaches might work better for exchanging drawing data in a chat interface?"

**Why it works:** This creates a deliberate pause for strategic thinking before committing to an implementation direction, often resulting in more robust architecture decisions.

### Format Redesign Request

**Pattern:** When facing fundamental limitations, request a reconceptualization rather than incremental fixes.

**Example:**

"Is it possible for you to simply generate the text, without rendering the image in the preview window?"

**Why it works:** This gives the AI permission to suggest more radical redesigns when appropriate, rather than being constrained to the current approach.

## Educational Enhancement Patterns

### Depth Over Brevity

**Pattern:** Request detailed explanations and comprehensive comments, even at the expense of conciseness.

**Example:**

"Please do a deep refactoring, focusing on learnability over optimization. I want to study what you've created."

**Why it works:** This shifts the AI from producing minimal, functional code to creating educational resources that illuminate the reasoning behind implementation choices.

### Structured Documentation Request

**Pattern:** Request specific documentation structures that serve educational purposes.

**Example:**

"Please create metadata comment headers at the top of the source code file containing enough context for me to be able to drop the source code into a new chat window and begin sketching."

**Why it works:** This creates standardized knowledge transfer mechanisms that make the codebase more accessible to newcomers and more valuable as a learning resource.

## Application-Specific Patterns

*(This section will grow as we discover patterns unique to specific types of applications.)*

### Vector Format Exchange

**Pattern:** Use simple JSON representations of visual elements rather than encoded bitmap images.

**Example:**

[SKETCH-DATA][{"x1":100,"y1":100,"x2":200,"y2":150,"width":5,"color":"black"}][/SKETCH-DATA]

**Why it works:** This creates a lightweight, human-readable format that can be easily transmitted in text-based interfaces while preserving the essential information about the drawing.

---

*Have you discovered effective prompt engineering patterns through your work? Consider contributing them to this document!*