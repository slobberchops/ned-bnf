# NES-BNF

Minimal BNF grammar for Dutch language.

## About

This project defines essential Dutch grammar rules using standard BNF (Backus-Naur Form) notation. **The goal is to cover A1-level Dutch** (CEFR beginner level) - the grammar needed for basic communication.

**A1 Level Target:**
- Simple present tense statements and questions
- Personal information (name, address, family, possessions)
- Basic greetings and introductions
- Numbers, time, dates
- Requests and commands (imperatives)
- Negation
- Common prepositions and locations
- Basic adjectives
- Simple past and future constructions

**Currently Defined:**
- ✓ Basic declarative sentences (subject-verb-object)
- ✓ Interrogative sentences with question words
- ✓ Personal pronouns (11 forms including clitics)
- ✓ Object pronouns (15 forms including clitics)
- ✓ Articles (de, het, een)
- ✓ Possessive pronouns (13 forms)
- ✓ Interrogative words (adverbs and pronouns)

**Still Needed for A1:**
- Verb conjugations (present tense)
- Adjectives and adverb placement
- Negation (niet, geen)
- Imperatives
- Numbers and time expressions
- Prepositions and prepositional phrases
- Basic past/future (heb + past participle, gaan + infinitive)
- Compound sentences with coordinating conjunctions (en, maar, want)

**Approach:**
- Minimal, not comprehensive - covers common constructs, not edge cases
- Enumerates closed word classes (pronouns, articles) as literals
- Uses lexical tokens (NOUN, VERB) for open word classes
- Handles Dutch-specific features: word order, determiners, interrogatives

## Supported Sentences

- Declarative: "ik ren", "ik zie je", "ik zie het huis", "het huis staat"
- Interrogative: "waar ligt het huis?", "wat is uw adres?"

## Grammatical Terms Glossary

### Sentence Types

**Declarative**: Statement sentence that declares/states something.
- Examples: "ik ren" (I run), "het huis staat" (the house stands)

**Interrogative**: Question sentence that asks something.
- Examples: "waar ligt het huis?" (where is the house?), "wat is uw adres?" (what is your address?)

### Sentence Components

**Subject**: Who/what does the action or is being described.
- Examples: "ik" in "ik ren", "het huis" in "het huis staat"

**Object**: Who/what receives the action.
- Examples: "je" in "ik zie je", "het huis" in "ik zie het huis"

**Determiner**: Word that specifies which/whose noun (articles, possessives).
- Examples: "de", "het", "een" (articles); "mijn", "uw", "zijn" (possessives)

**Adverb**: Word that modifies a verb, adjective, or another adverb, describing how, when, where, or to what extent.
- Interrogative adverbs: "waar" (where), "wanneer" (when), "hoe" (how), "waarom" (why)