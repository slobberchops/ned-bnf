# Development Workflow

## Markdown Formatting

### Line Length

- **NEVER** exceed 99 characters per line in markdown files
- Break long sentences at natural points (after punctuation, conjunctions, or logical breaks)
- Use soft line breaks within paragraphs to maintain readability in editors
- Code blocks, mermaid diagrams, and URLs are exempt from line length limits

### Examples

✅ **Good (proper line breaks):**

```markdown
This is an extremely long line that exceeds the 99 character limit and should be broken up into
multiple shorter lines for better readability and consistency with our style guide.
```

✅ **Good (natural break points):**

```markdown
When a sub-module imports from a sibling package, all parent packages up to (but not including) the
common ancestor inherit that dependency relationship.
```

### Rationale

- Improves readability in editors and diff views
- Makes collaborative editing easier
- Maintains consistency across all project files

## Commit Message Style

You can either write detailed commit messages by hand, but it is recommended that you use the
project commit message generation tools via claude.

### Structure

- Use a clear, concise subject line (50 characters or less)
- Leave a blank line between subject and body
- Organize the body into sections with bullet points
- End with generation attribution
- Only include sections if relevant

### Sections

Use these sections as appropriate:

**Changes:**

- List specific modifications made
- Focus on what was changed, not why

**Features:**

- New functionality added
- Enhancements to existing features

**Fixes:**

- Bug fixes and corrections
- Issues resolved

**Tests:**

- New test cases added
- Test improvements or modifications

**Refactoring:**

- Code restructuring without functional changes
- Performance improvements

### Example

```
Add Resource.get decorator with comprehensive testing

Changes:
- Add get decorator method to Resource class
- Implement read-only get_handler property
- Add error handling for unregistered handlers

Tests:
- Add test for decorator registration functionality
- Add test for read-only property behavior
- Add test for AttributeError when handler not set
```

### Rationale

- Structured format improves readability
- Bullet points make changes easy to scan
- Consistent sections help with code review
- Clear separation between different types of changes
