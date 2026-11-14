---
name: convert-document
description: Convert supported PDF, Word, Excel, PowerPoint, HTML and other documents to Markdown through MarkItDown MCP.
---

# Convert documents with MarkItDown

When asked to convert a supported document, use the MarkItDown MCP tool `convert_to_markdown` with an accessible URI.

1. Verify the file or URI is supplied and accessible. Ask for a path when missing.
2. For local files, use the appropriate file URI accepted by the MCP server.
3. Call the MCP conversion tool; do not pretend conversion succeeded if the tool is unavailable.
4. Return the Markdown, retaining headings, links and tables where supported.
5. Clearly identify missing images, OCR limitations or formatting loss.

Do not read unrelated files, fetch untrusted URLs, or transmit confidential documents to external services without authorization.
