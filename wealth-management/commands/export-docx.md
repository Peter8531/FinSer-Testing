---
description: Export the most recent Strategy Request to a Word document (.docx)
argument-hint: "[input.md] [output.docx]"
---

Export a Strategy Request markdown file to a formatted Word document (.docx) using the export script.

Run: `python3 wealth-management/scripts/export_docx.py <input.md> [output.docx]`

If no input file is specified, look for the most recently modified `.md` file in `wealth-management/output/`. If no output path is specified, the `.docx` is written alongside the input file.

The exported document includes:
- Formatted tables with styled headers (dark blue background, white text)
- Calibri font throughout, narrow margins
- Footer: "SOA Summary Request - Internal Working Paper - Not for Client Distribution"
- Automatic row-number column removal for cleaner tables
- Section headings matching the Strategy Request template

Requires `python-docx` (`pip install python-docx`).
