# Endpoint Status

**Widgets for [Gatus](https://github.com/TwiN/gatus)** — your self-hosted
fleet's health on the iPhone Home Screen and Lock Screen.

An unofficial, third-party client. Not affiliated with, endorsed by, or
supported by the Gatus project.

## What it does

- **Home Screen widgets** — small, medium and large: how many endpoints are up,
  and which are down.
- **Lock Screen widgets** — circular, rectangular and inline.
- **Live Activity** — during an outage, a Lock Screen card and Dynamic Island
  presentation showing which endpoint is down and for how long, counting live.
  It arms itself when the app is open and something is failing.
- **Endpoint detail** — recent probe history, uptime over the retained window,
  the conditions that failed, and when the current outage began.

## Requirements

A [Gatus](https://github.com/TwiN/gatus) instance you can reach from your
iPhone. Gatus's status API needs no account, so there is nothing to sign in to —
you only enter the instance's address.

Plain `http://` works for the usual self-hosted shapes: an IP address
(`http://192.168.1.10:8080`), a `.local` name, or an unqualified hostname.
Cleartext to a *public* domain is blocked by iOS and will not work; use HTTPS
for anything reachable from the internet.

No instance yet? The app offers the Gatus project's own public dashboard at
`status.twin.sh` as a one-tap way to try it.

## Support

Questions, bugs and feature requests: **[open an issue](https://github.com/peterlvilim/endpoint-status/issues)**.

Please include your iOS version and, if relevant, your Gatus version — the
status API's shape has changed between releases before.

## Privacy

Endpoint Status collects nothing. See [PRIVACY.md](PRIVACY.md).
