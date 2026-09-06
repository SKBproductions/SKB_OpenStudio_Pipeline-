# Security Guidelines

This is a public repository. Do not commit:

- Passwords, API keys, access tokens, or recovery codes
- A populated `.env` file
- Unreleased scripts, private character references, or business records
- Licensed source media that SKBproductions cannot redistribute
- Large local ComfyUI models, caches, or production outputs

## Credential handling

Keep real credentials in a local `.env` file or an approved encrypted secret store. Code should read credentials from environment variables. Credentials must never appear in browser-side HTML, prompts, screenshots, filenames, logs, or commit messages.

If a credential is exposed, revoke it at the service provider immediately, create a replacement, and review repository history before continuing.

## Paid generation safety

Future Runway, Pika, or other paid integrations should require explicit approval before starting a batch. Set spending controls with the provider whenever available.

## ComfyUI safety

Keep a local ComfyUI server bound to `127.0.0.1` unless remote access has been deliberately secured. Do not expose an unauthenticated ComfyUI instance directly to the public internet.

## Reporting

Security concerns involving this repository should be reported privately to SKBproductions, LLC rather than posted with sensitive details in a public issue.
