# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a **D&D campaign documentation repository**, not a software project. It contains campaign notes and encounter information stored as Microsoft Word documents (.docx format).

## Repository Structure

The repository uses a flat structure with character-specific campaign notes and shared resources:

- **Christophers Path. .docx** - Campaign notes for Christopher's character
- **Lena'a Path.docx** - Campaign notes for Lena's character
- **Nicks Path.docx** - Campaign notes for Nick's character
- **Encounters all.docx** - Shared encounter details and reference material

## Working with .docx Files

**Important Limitations:**
- .docx files are binary formats (ZIP archives containing XML) and cannot be directly read or edited by Claude Code's text-based tools
- To view or modify content, users must open these files in Microsoft Word, LibreOffice Writer, Google Docs, or similar software
- Changes to .docx files must be made externally and then committed to git

**When users request changes to campaign notes:**
1. Inform them that .docx files must be edited in Word or compatible software
2. After external edits, help commit and push changes if requested
3. For significant content additions, suggest creating new markdown (.md) files as a text-based alternative

## Git Workflow

**Current Branch:** `claude/init-project-01CKmsjNXb4b8DhXNjYe9T8J`

**Common Operations:**
```bash
# Check status
git status

# Commit changes after external document edits
git add "Christophers Path. .docx"  # Note: filename has space and double extension
git commit -m "Update Christopher's campaign notes"

# Push to remote
git push -u origin claude/init-project-01CKmsjNXb4b8DhXNjYe9T8J
```

**Note on Filenames:**
- Some files contain spaces and special characters (e.g., "Christophers Path. .docx" has double extension)
- Always quote filenames in git commands to handle spaces properly

## Repository Purpose

This repository serves as collaborative storage for a D&D campaign, allowing multiple players to track their individual character paths and share common encounter information. It's version-controlled to maintain history of campaign progression and allow rollback if needed.

## Recommendations for Future Enhancements

If users want Claude Code to help manage campaign content more effectively:
- Consider adding markdown (.md) files for text-based notes that Claude can read and edit
- Create a README.md to document the campaign setting, active characters, and session history
- Add a changelog or session log in markdown format to track campaign events
