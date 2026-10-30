# TruHuddle documentation

This repository contains the public customer documentation built with Mintlify. Configuration is in docs.json and pages are MDX with title, description and keywords.

## Product and audience

- TruHuddle is an organization blogging service. Use workspace, blog, article, Startup and Enterprise consistently.
- Write for workspace owners, editors and developers integrating the published-content API.
- The source application is https://github.com/retinaNigeria/theretinalabs, directory truhuddle. Verify behavior against current source before changing API examples or plan limits.
- This repository is deployed separately from the application. Never copy application environment files or credentials here.

## Style and branding

- Use active voice, second person, sentence case and concise instructions.
- Use the existing #0287fd brand blue, League Spartan typography and unmodified TruHuddle logo.
- Use Markdown code fences with language tags for syntax highlighting.
- Prefer built-in Mintlify components; keep navigation simple and omit unnecessary icons.
- Keep every page linked from docs.json and internal links root-relative without file extensions.

## Boundaries

- Document customer features, public API usage and customer-managed custom-domain Workers.
- Never document internal control-room access, private endpoints, platform gateway secrets, database schemas or infrastructure credentials.
- API examples use placeholders only. Requests are server-side, read-only and Enterprise-scoped.
- Do not promise that AI output is always correct or that prompt injection can be eliminated.
- Do not reintroduce newsletter or email-list features. They were removed.

## Workflow

Read the Mintlify skill and run mint instructions for current platform guidance. Check MDX, docs.json and internal links after changes. Do not run authenticated app requests, paid AI calls or database modifications to validate documentation. Push only when authorized and never claim a deployment is live without verifying its status.
