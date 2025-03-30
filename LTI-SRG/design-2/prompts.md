# Prompt para Claude utilizando el modelo 3.7 para hacer meta prompting

As an expert in prompt engineering and using all best practices in prompting, improve this statement to meet all requirements. "Using the documents in the *design-1* section that make up a basic PRD (key functionalities, use cases, data model, etc.), your mission is to prepare the necessary documentation to begin implementing LTI:
* **Generate User Stories.** You can create as many as you want and can, with a minimum of two. Use the best practices learned in this chapter to ensure they contain all necessary information. As a recommendation, use a common template for all of them (remember that an example template is provided in the *User Stories* section).
* **Build the product backlog** with the User Stories, prioritizing them as you see fit according to a specific methodology. Experiment with different ways to generate a prompt that can create your backlog based on the documentation you've prepared. Provide the different prompts you used and indicate which one gave the best results. Along with the prompts, include your conclusions on why you think that specific prompt was effective.
* **Choose your preferred User Story** and generate work tickets. Define them technically, just as it is done in planning meetings.
* **Estimate the effort** required for the work tickets using the methodology (Fibonacci, Planning Poker, T-shirt sizes) and units (hours, story points) of your choice.
* **Document everything in a single file** named *UserStories-SRG.md*."

# Prompt para Cursor utilizando Claude 3.7 en modo agent

# LTI Implementation Documentation Task

## Context
Using the comprehensive PRD documents in the *design-1* section (including key functionalities, use cases, and data model), prepare all necessary documentation to begin implementing the LTI integration.

## Tasks

### 1. Generate User Stories (Required)
- Create a minimum of 5 comprehensive user stories that cover core LTI functionality
- Follow the industry-standard template: "As a [user role], I want to [action/feature] so that [benefit/value]"
- Include acceptance criteria for each story (minimum 3 criteria per story)
- Ensure each story is independent, negotiable, valuable, estimable, small, and testable (INVEST principles)
- Tag each story with appropriate categories (e.g., Authentication, Content Management, Analytics)

### 2. Build the Product Backlog
- Prioritize all user stories using the MoSCoW method (Must have, Should have, Could have, Won't have)
- Include rationale for each prioritization decision
- Document your prompt engineering process:
  * Provide 3 distinct prompts you used to generate the backlog
  * For each prompt, explain your reasoning and methodology
  * Analyze the results and explain which prompt was most effective and why
  * Include specific elements that made the winning prompt superior (specificity, context, instruction clarity, etc.)

### 3. Generate Technical Work Tickets
- Select your highest-priority user story
- Break it down into 4-6 discrete technical tasks
- For each task, include:
  * Clear title
  * Technical description with implementation details
  * Definition of Done criteria
  * Dependencies and related tickets
  * Technical constraints or considerations

### 4. Estimate Implementation Effort
- Apply Fibonacci sequence story point estimation (1, 2, 3, 5, 8, 13, 21)
- Provide justification for each estimate based on complexity, uncertainty, and effort
- Include a brief explanation of your estimation methodology
- Add a summary table showing total estimated points

### 5. Documentation Deliverable
- Compile all information into a single well-structured Markdown file named *UserStories-SRG.md*
- Include a table of contents at the beginning
- Use proper Markdown formatting (headers, lists, tables, code blocks) for readability
- Add an appendix explaining any assumptions made during the process