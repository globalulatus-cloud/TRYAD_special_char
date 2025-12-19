Japanese Punctuation Validator and Annotator (Streamlit App)

This Streamlit application validates and normalizes Japanese punctuation in Excel files by comparing the target Japanese text against a source English column. It automatically fixes half-width characters, detects missing or extra punctuation, and annotates reasons for each change.

Features

Upload Excel (.xlsx) files via browser UI

Automatically converts half-width characters to full-width Japanese punctuation

Validates punctuation consistency against the source text

Adds two new columns:

Fixed Japanese

Reason for Change / Validation

Supports multiple sheets in a single Excel file

Download the validated Excel file instantly

No data is stored on the server

Supported Punctuation Rules

The app currently validates and fixes the following characters:

Half-width	Full-width
(	（
)	）
[	［
]	］
,	、
/	／
.	。
X	×
:	：
#	＃
Expected Excel Format
Column	Description
A	Source text (English)
B	Target text (Japanese)
C	Fixed Japanese (auto-generated)
D	Reason for Change / Validation (auto-generated)

Notes:

Columns C and D are created or overwritten by the app.

Non-string cells are safely ignored.

All sheets in the workbook are processed.
