<div align="center">

### Connect your VPN without ever typing a one-time code again.

**[PassTunnel](https://github.com/PassTunnel/passtunnel)** is an open-source macOS app for OpenVPN and FortiGate SSL VPN.
It keeps your TOTP secret in the Keychain and fills in the current code (and your password) every time you connect.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/PassTunnel/passtunnel/main/docs/images/main-dark.png">
  <img src="https://raw.githubusercontent.com/PassTunnel/passtunnel/main/docs/images/main-light.png" width="600" alt="PassTunnel main window with live one-time codes">
</picture>

[Download](https://github.com/PassTunnel/passtunnel/releases/latest) ·
[Install with Homebrew](https://github.com/PassTunnel/passtunnel#install) ·
[Use with AI assistants](https://github.com/PassTunnel/passtunnel#use-with-ai-assistants-mcp) ·
[Security](https://github.com/PassTunnel/passtunnel/blob/main/SECURITY.md)

</div>

- **Menu bar app and CLI** in one signed, notarized binary, with Touch ID protection for your secrets.
- **MCP server for AI assistants.** `passtunnel mcp` lets Claude Code, Claude Desktop and other MCP clients
  check your VPN, read its logs and diagnose problems; with `--allow-connect` they can also connect and
  disconnect. It never returns passwords, TOTP secrets or codes.
- **Scriptable.** `--json` on every command, stable exit codes, non-interactive flags
  ([docs/CLI-JSON.md](https://github.com/PassTunnel/passtunnel/blob/main/docs/CLI-JSON.md)).

```sh
brew trust passtunnel/tap && brew install --cask passtunnel/tap/passtunnel
claude mcp add -s user passtunnel -- passtunnel mcp
```
