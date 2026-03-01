# NED-BNF

Minimal BNF grammar for Dutch language.

---

# [`nederlands.bnf`](./nederlands.bnf)

---

## About

BNF grammar for A1-level Dutch (CEFR beginner) - the grammar needed for basic communication.

**What works now:**
- Declarative and interrogative sentences (subject-verb-object, question words)
- Pronouns: personal, object, possessive, interrogative
- Articles: de, het, een
- Negation: niet (negative adverb), geen (negative article)

**Still needed:**
- Verb conjugations (present tense)
- Adjectives and adverbs
- Imperatives
- Numbers and time
- Prepositions
- Past/future (heb + participle, gaan + infinitive)
- Conjunctions (en, maar, want)

**Approach:**
- Minimal, not comprehensive
- Closed word classes (pronouns, articles) listed as literals
- Open classes (nouns, verbs) as tokens
- Handles Dutch word order and determiners

## Understanding the Grammar Rules (BNF Notation)

The grammar rules in this project are written in **BNF** (Backus-Naur Form), a notation
originally made for computer nerds to precisely describe programming languages. But it uses
simple symbols, so maybe normal people can read it too. Think of it as a recipe that shows how
to build valid Dutch sentences.

**How to read the rules:**

- `<sentence>` - A grammar concept (like "sentence" or "subject") - written in angle brackets
  and English
- `::=` - Means "is made from" or "consists of"
- `"ik"` - An actual Dutch word that appears in quotes
- `|` - Means "or" - shows alternative options
- `[...]` - Means optional - you can include this or skip it
- `{...}` - Means you can repeat this part multiple times
- `VERB` - A placeholder for any word of that type
- `//` - Starts a comment (explanation note)

**Simple example:**
```
// A sentence is made from: a subject, then a verb, and optionally an object
<sentence> ::= <subject> <verb> [<object>]

// A subject can be "ik" or "jij" or a noun phrase
<subject> ::= "ik" | "jij" | <noun_phrase>

// A verb can be any Dutch verb word
<verb> ::= VERB
```

This means "ik ren" (I run) is valid, and "ik zie je" (I see you) is also valid because the
object is optional.

**Learn more:** [Backus-Naur Form on Wikipedia](https://en.wikipedia.org/wiki/Backus%E2%80%93Naur_form)

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

**Adverb**: Word that modifies a verb, adjective, or another adverb, describing how, when,
where, or to what extent.
- Interrogative adverbs: "waar" (where), "wanneer" (when), "hoe" (how), "waarom" (why)

**Determiner**: Word that specifies which/whose noun (articles, possessives).
- Examples: "de", "het", "een" (articles); "mijn", "uw", "zijn" (possessives)

**Object**: Who/what receives the action.
- Examples: "je" in "ik zie je", "het huis" in "ik zie het huis"

**Pronoun**: Word that replaces a noun or noun phrase.
- Personal pronouns: "ik" (I), "jij" (you), "hij" (he), "zij" (she)
- Object pronouns: "mij" (me), "jou" (you), "hem" (him), "haar" (her)
- Possessive pronouns: "mijn" (my), "jouw" (your), "zijn" (his), "haar" (her)
- Interrogative pronouns: "wat" (what), "wie" (who)

**Subject**: Who/what does the action or is being described.
- Examples: "ik" in "ik ren", "het huis" in "het huis staat"