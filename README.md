# Mailganer Agent Inbox (hosted MCP)

Temporary inbox for AI agents. Get an address and a Bearer on the tools page, then call `wait_for_code`. No MX, no SMTP.

**Homepage:** https://mailganer.com/tools/agent-inbox

Not Email OTP Verify (https://mailganer.com/tools/email-otp) — that sends a code to *your* users.

## Install in Cursor

1. Open https://mailganer.com/tools/agent-inbox → **Get inbox**.
2. Copy the Bearer `aib_…` (session ~2 hours). Do not commit it.
3. Set `AGENT_INBOX_TOKEN` to that value, or paste the JSON from the page into `mcp.json`.

This repo’s `.mcp.json` is the Cursor Directory listing. The live `mcp_url` from allocate on apex may still be `https://mailganer.com/tools/email-otp/v1/inbox/mcp` (same process). Alias: `https://mailganer.com/tools/agent-inbox/v1/mcp`.

## Tools

`get_inbox`, `list_messages`, `wait_for_code`, `get_message`, `mark_read`, `burn_inbox`

Compatibility with a given signup form is not guaranteed.
