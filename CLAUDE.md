# Mnemosyne — Claude Instructions

This is a personal knowledge base maintained by Claude Code using the LLM Wiki pattern.
Focus areas: AI/LLM research, bookmarks, tools, and techniques.

## Workflow

### Processing inbox
When asked to process inbox:
1. Read every file in `inbox/`
2. For each item, decide: concept note, tool note, or source note
3. Write the note into the appropriate `wiki/` subfolder using the template in `_templates/`
4. Add backlinks to related existing wiki notes (`[[note-name]]` syntax)
5. Move the processed inbox file to `.trash/` (or delete it)
6. Append a one-line entry to the log in `index.md`: `- YYYY-MM-DD: processed N items`

### Writing concept notes (`wiki/concepts/`)
- Title = the concept name, kebab-case filename
- Summary: 2-3 sentences in plain language
- Key Ideas: bullet points, concrete and specific
- Related: wikilinks to other concept/tool notes

### Writing tool notes (`wiki/tools/`)
- What it is, who makes it, what problem it solves
- Link to relevant concepts it implements

### Writing source notes (`wiki/sources/`)
- Preserve the URL
- Summarize what's worth remembering, not everything
- Extract concepts and link them

### Synthesis (`wiki/synthesis/`)
- Only write these when asked
- Cross-concept essays: "how X and Y relate", "state of X as of date"

## Style
- Write in second person ("you") when explaining concepts to the reader
- Be concise — notes should be scannable, not exhaustive
- Prefer wikilinks over repeating explanations
- No filler phrases ("it's worth noting", "importantly")
