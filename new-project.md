You are helping the user start a new project. Follow these steps in order:

## Step 0: Project folder
First, before anything else, ask the user:
"האם יש לך כבר תיקייה לפרויקט?"
- If yes: ask for the full path and use it as the working directory.
- If no: ask for (1) the folder name, (2) where to create it. Then create the folder.

## Step 1: Understand the project
Ask the user to describe the project idea. Ask clarifying questions if needed:
- What is the goal?
- What tech stack (or should you recommend one)?
- Where will it run (local / cloud)?
- Any cost constraints (free only)?

## Step 2: Create CLAUDE.md
Once you have enough information, create a CLAUDE.md file in the project directory with:
- Project overview
- Tech stack
- Goals and phases
- Environment variables needed
- Security constraints (if any)

## Step 3: GitHub setup
Always offer to set up a GitHub repository for backup and deployment. Ask:
- Do you have a GitHub account?
- Should the repo be public or private?
Then guide the user to create the repo and connect it locally.

## Step 4: Project structure
Create the minimal folder structure needed to get started. Do not over-engineer.

## Step 5: Save to memory
Save any important decisions or preferences discovered during this conversation to MEMORY.md.

---

Rules:
- Never ask for tokens, API keys, or passwords in chat. Always direct the user to enter them directly in the relevant service (Railway, .env file, etc.)
- ALWAYS number all options (1, 2, 3...) so the user can choose easily. Never present options without numbers.
- Keep explanations simple - the user is not a developer
- Respond in Hebrew
