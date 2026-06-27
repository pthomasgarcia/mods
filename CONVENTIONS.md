# Git Commit Message Conventions

## GPG Signing Workflow

This repository requires GPG-signed commits. Aider cannot execute signed commits directly, so use the following handoff process for all changes:

1. **Do Not Attempt Direct Commits:** Never run `git commit` or any git commit API call.
2. **Use the Handoff File:** Write the commit message to `.gitmessage` in the project root, overwriting any existing content.
3. **Format and Scope:**
   - A concise imperative summary line (max 50 chars)
   - A blank line
   - A detailed bulleted body explaining *what* was changed and *why*
4. **User Execution:** The user will review `.gitmessage` and execute the signed commit manually.
