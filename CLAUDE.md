# Engram — Claude Instructions

This is a personal knowledge base maintained by Claude Code using the LLM Wiki pattern.
Focus areas: AI/LLM research, bookmarks, tools, and techniques.

## Workflow

### Processing inbox
When asked to process inbox:
1. Read every file in `inbox/`
2. If the file is a Chrome/Brave HTML bookmark export (contains `<!DOCTYPE NETSCAPE-Bookmark-file-1>`), parse all `<A HREF=...>` tags to extract URLs and titles — treat each as a bookmark to process
3. For each item/bookmark, decide: concept note, tool note, or source note
4. Write the note into the appropriate `wiki/` subfolder using the template in `_templates/`
5. Add backlinks to related existing wiki notes (`[[note-name]]` syntax)
6. Delete the processed inbox file
7. Append a one-line entry to the log in `index.md`: `- YYYY-MM-DD: processed N items`

### Importing browser bookmarks
To export from Chrome or Brave: Bookmarks Manager → ⋮ menu → Export bookmarks → save HTML file into `inbox/`.
When processing a bookmark HTML export:
- Skip bookmarks that are folders, separators, or have no meaningful title
- Group related bookmarks into a single source note if they're about the same topic rather than making one note per link
- For AI/LLM bookmarks: prefer tool notes for products/services, concept notes for papers/techniques, source notes for articles

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

### Seeding from external repos
To seed the wiki from a public GitHub repo:
1. Fetch the repo's content via `https://raw.githubusercontent.com/<owner>/<repo>/main/<path>`
2. Filter to AI/LLM topics only
3. Map each item: techniques/papers → concept, frameworks/services → tool, articles/surveys → source
4. Deduplicate against existing wiki notes before writing
5. Write notes using templates in `_templates/`
6. Update `index.md` log

Repos used as seeds: Hannibal046/Awesome-LLM, NicholasSpisak/second-brain (2026-05-14)

## Style
- Write in second person ("you") when explaining concepts to the reader
- Be concise — notes should be scannable, not exhaustive
- Prefer wikilinks over repeating explanations
- No filler phrases ("it's worth noting", "importantly")
