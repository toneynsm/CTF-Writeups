# CLAUDE.md - CTF Writeups Repo

This file tells Claude how to work in this repository.

---

## Repo Structure

```
CTF-Writeups/
├── README.md                        # Root index (update challenge counts when adding writeups)
├── CLAUDE.md                        # This file
├── Web-Exploitation/
│   ├── README.md                    # Category index table
│   └── challenge-name.md            # One file per challenge
├── Cryptography/
├── Reverse-Engineering/
├── Forensics/
├── General-Skills/
├── Binary-Exploitation/
└── Blockchain/
```

File names: lowercase, hyphenated (e.g., `cookie-monster-secret-recipe.md`).

---

## Writeup Format

Every writeup follows this exact structure:

```markdown
# Challenge Name

| Field | Details |
|-------|---------|
| Platform | PicoCTF / HTB / CTFtime / etc. |
| Category | Web Exploitation / Cryptography / etc. |
| Status | Solved |

---

## Summary
One sentence: what the challenge was and how it was solved.

## Approach
Numbered steps of exactly what was done. Include commands, payloads, and tool names.

## Vulnerability
Technical explanation of the flaw: what was broken and why.

## Key Takeaways
- Lessons learned
- Defensive mitigations
- Real-world relevance
- OWASP / MITRE ATT&CK references where applicable

---

*[← Back to Category](README.md)*
```

---

## When Adding a New Writeup

1. Create the `.md` file in the correct category folder using the format above.
2. Add a row to the category `README.md` table.
3. Update the challenge count for that category in the root `README.md`.
4. Commit with message: `add writeup: [Challenge Name] ([Category])`
5. Push to GitHub.

---

## Git Workflow

- Branch: `main`
- Remote: `origin` (GitHub)
- Commit style: `add writeup: Head Dump (Web Exploitation)`
- Always push after adding or editing writeups.

---

## User Context

- Platform focus: PicoCTF (primary), others as encountered
- The user is building this repo to document CTF progress and reinforce security concepts
- Writeups should be readable to someone learning. Explain the "why", not just the "what"
- Include real-world context and MITRE/OWASP references where relevant
