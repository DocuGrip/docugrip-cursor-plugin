# DocuGrip for Cursor

Find the right PDF tool, official upload limits and official forms, with the link to do it.

This plugin connects Cursor to the DocuGrip MCP server at `https://docugrip.com/api/mcp`.
Describe a PDF task in plain language ("compress this to under 2 MB", "turn these photos into a PDF",
"black out account numbers") and the assistant returns the right DocuGrip tool and the page to open.

## Tools

| Tool | What it does |
|---|---|
| `list_pdf_tools` | Lists DocuGrip's PDF tools by family |
| `find_pdf_tool` | Finds the right tool for a task described in plain language |
| `plan_pdf_job` | Turns a job with several steps into ordered steps with their pages, the runs it takes, and the plan that fits when it needs more than the daily allowance |
| `get_pdf_tool` | Details and link for one tool |
| `get_upload_requirements` | Official upload limits of 50 portals and services — IRCC, USCIS, Gmail, LinkedIn, UCAS and more — with sources |
| `find_official_form` | Finds official forms such as W-9, 1099-NEC or I-130, with the current edition |
| `get_plans` | Current plans and prices, with direct links |

All tools are read-only. No API key, no sign-in, no configuration. The server never receives, opens or
stores a document; it returns links to docugrip.com, where the work happens.

## Install

Install from Cursor's plugin list, or add the server yourself in `~/.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "docugrip": { "url": "https://docugrip.com/api/mcp" }
  }
}
```

## Links

- Server page: https://docugrip.com/mcp-server
- Privacy: https://docugrip.com/privacy
- Terms: https://docugrip.com/terms
- Support: hello@docugrip.com

The files in this repository are MIT licensed. The DocuGrip name and logo are trademarks of
Simulator Arts LLC and are not covered by the license.
