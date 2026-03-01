# NED-BNF Project

## Project Purpose

This project defines a minimal BNF (Backus-Naur Form) syntax for the Dutch language.

## Guidelines

- Focus on minimal, essential grammar rules for Dutch
- Use standard BNF notation conventions
- Keep definitions clear and unambiguous
- Consider Dutch-specific features: word order, compound words, separable verbs
- Prioritize common language constructs over edge cases

## BNF Notation

- Use `//` for comments
- Use `::=` for definitions
- Use `|` for alternatives
- Use `< >` for non-terminals (in English)
- Use `" "` for terminals/literals (in Dutch)
- Use `UPPERCASE` for lexical token markers (e.g., VERB, NOUN, PRONOUN)
- Use `[ ]` for optional elements
- Use `{ }` for repetition (zero or more)
- Non-terminal names (left-hand side) are written in English
- Terminal values (right-hand side literals) are in Dutch
- Lexical categories (word classes) are represented by uppercase markers rather than enumerating all words
- Long comments (descriptive, with examples) go above the rule, not inline
- Limit lines to 80 characters