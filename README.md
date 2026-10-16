# Matchall for ChatGPT

Public source preparation for the Matchall ChatGPT plugin. **Not submitted to or
approved by the ChatGPT plugin directory.** The manifest version identifies this
source package; no GitHub release or marketplace version has been published.

## Package and installation path

This repository uses Agent Plugins 1.0: root `plugin.json`, `mcp.json`, and
`skills/match-service/SKILL.md`. The manifest uses the `matchall-chatgpt`
name and includes OpenAI listing metadata plus five positive and three
negative review cases.

Build the ZIP using the commands below. An authorized developer can later upload
it as a draft through the OpenAI plugin submission portal, configure the remote
OAuth connection, and run the review cases. A GitHub upload does not install the
plugin into ChatGPT or replace an existing private installation. This package is
**not submission-ready**; missing listing and review items are tracked below.

## What Matchall does

Draft needs and offers in natural language, activate them after approval, inspect
matches, and exchange private contact details only with mutual consent. Pause or
close needs when appropriate. Match scores do not guarantee transactions;
Matchall does not place orders or process payments.

## Authorization and data

The remote MCP endpoint is `https://awiki.info/amatch/v2`.
Use the host's OAuth connection UI. Discovery advertises PKCE S256, dynamic
client registration, and `intent:read` / `intent:write` scopes. Never put tokens,
passwords, verification codes, or private contact details in this repository.
Do not configure shared secret headers as an OAuth workaround.

Email binding is optional and helps with account recovery and notifications.
Private contact details are entered separately from business text and login
email. Without email, use manual checks or a host-supported scheduled task.
A schedule is not created merely by installing this plugin.
Business text is processed by the hosted Matchall service and its configured
model providers. This repository is the client plugin package, not the backend.

## Example prompts

- “Draft a need for five standing desks in Singapore. Show me before activating.”
- “Show current matches and explain which product fits have been verified.”
- “Ask this matched supplier to exchange contact details after showing me mine.”
- “Pause my standing-desk need; keep it for later.”

## Development

```sh
python3 -m venv .venv
. .venv/bin/activate
python -m pip install -r requirements-dev.txt
python scripts/validate.py
python scripts/package.py
```

The validator checks package structure, referenced assets, contact workflow,
review case inventory, and absence of embedded credentials. ZIP generation is
local only, uses an explicit file allowlist, and inspects the generated archive.
Neither script installs a plugin, invokes matching tools, deploys the service,
or submits a marketplace application. CI only validates and packages locally.
See [readiness](docs/READINESS.md) for the remaining marketplace work.

## Support and license

Use this repository's Issues for public package bugs. Never post credentials,
private contact details, or account recovery information in issues. A dedicated
private service-support channel and service policies are still being prepared.

[MIT](LICENSE) applies to this plugin package. It does not grant access to other
users' data, relicense the hosted backend, or imply permission to impersonate
AWiki, Matchall, OpenAI, Cursor, or xAI. The monochrome logo follows AWiki branding.

## Matchall naming transition

The plugin is now named `matchall-chatgpt` and the MCP connection label is
`matchall`. Its source repository is now
[AgentConnect/matchall-chatgpt](https://github.com/AgentConnect/matchall-chatgpt).
The existing OAuth/MCP URLs are unchanged; renaming the display/package does not
migrate accounts or change permissions.
This source update does not publish a release or update installed host copies.
