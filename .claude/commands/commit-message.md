Print a concise commit message for the current staged and unstaged changes using the commit message
style from STYLE.md in the project root.

Follow this process:

1. Run `git status --porcelain` and `git diff --cached` and `git diff` to understand the current
   changes
2. Analyze the changes to categorize them (Changes, Features, Fixes, Tests, Refactoring)
3. Create a commit message following this structure:
   - Clear, concise subject line (50 characters or less)
   - Blank line
   - Organized sections with bullet points (only include relevant sections)
   - End with generation attribution

Only include sections that are relevant to the changes. Focus on what was changed, not why. Do not
include basic steps that accomplish the ultimate goal, such as commenting on new imports and adding
type information.
