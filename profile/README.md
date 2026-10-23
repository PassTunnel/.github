<div align="center">

### Connect your VPN without ever typing a one-time code again.

**[PassTunnel](https://passtunnel.github.io/)** is a free, open-source macOS app for OpenVPN and FortiGate SSL VPN.
It keeps your TOTP secret in the macOS Keychain, computes the current code and sends it with your password when you click Connect.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://passtunnel.github.io/assets/img/main-dark@2x.webp">
  <img src="https://passtunnel.github.io/assets/img/main-light@2x.webp" width="640" alt="PassTunnel main window: each VPN profile with its live one-time code and countdown ring">
</picture>

**[Website](https://passtunnel.github.io/)** ·
[Download for Mac](https://github.com/PassTunnel/passtunnel/releases/latest/download/PassTunnel.dmg) ·
[Install with Homebrew](https://passtunnel.github.io/#install) ·
[CLI & MCP](https://passtunnel.github.io/#cli) ·
[Security](https://github.com/PassTunnel/passtunnel/blob/main/SECURITY.md)

<sub>macOS 13+ · Apple silicon · Free & open source (MIT)</sub>

</div>

- **One-time codes, handled.** Sent in whatever format your server expects; with fewer than 8 seconds left
  in the code window, PassTunnel waits for a fresh code. QR import, optional Touch ID per profile.
- **A complete VPN client.** Signed `openvpn` and `openfortivpn` bundled, menu bar badges per profile,
  auto-reconnect, several VPNs at once, shareable profiles without secrets.
- **CLI & MCP.** The `passtunnel` CLI with `--json` and stable exit codes; `passtunnel mcp` lets Claude Code,
  Claude Desktop, Cursor, VS Code and other MCP clients check status, read logs and diagnose problems.
  Read-only by default, and it never hands out passwords, secrets or codes.
- **Your secrets stay on your Mac.** Login Keychain without iCloud sync, a privileged helper approved once
  instead of an admin password at every connect, Developer ID signed and notarized.

```sh
brew trust passtunnel/tap
brew install --cask passtunnel/tap/passtunnel
```
