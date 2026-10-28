# Workflows

Export your own workflows from n8n (three-dot menu > Download) and save them here:

- `kb-ingestion-v1.json` : upload form > extract text > chunk > embed > vector store
- `support-agent-v2.json` : chat trigger > AI agent + knowledge base tool

Before committing, confirm no API key is inside:

    grep AIza *.json          # Mac / Linux
    findstr /i "AIza" *.json  # Windows

n8n stores credentials separately from workflow JSON, but always check.
