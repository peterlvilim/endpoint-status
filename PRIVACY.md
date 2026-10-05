# Privacy Policy — Endpoint Status

_Last updated: 5 October 2026_

**Endpoint Status collects nothing.**

There is no analytics, no crash reporting, no advertising, no tracking, and
no account. The app has no backend of its own, and the developer operates no
server that it talks to.

## What the app stores

Three things, all on your device, in the app's own App Group container shared
with its widget extension:

- the URL of the Gatus instance you choose,
- whether you want outages to raise a Lock Screen card automatically,
- a cached copy of the most recent status it fetched, so widgets can render
  when a refresh fails.

None of it leaves your device. Deleting the app deletes all of it.

## What the app sends, and to whom

Endpoint Status makes HTTP requests to **the Gatus instance you configure, and
to nothing else**. Those requests go to a server you chose — normally your own.
The developer cannot see them.

Gatus's status API is unauthenticated, so the app holds no password, token or
API key for it.

If you tap **Use the public demo instance** on first launch, the app will read
from `status.twin.sh`, a public Gatus dashboard operated by the Gatus project
and not by the developer of this app. It is offered so the app can be tried
without a server of your own. Whatever that instance logs about requests is
governed by its operator, not by this policy. You can change the instance at
any time from the Instance screen.

## Required-reason API disclosure

The app accesses `UserDefaults` (Apple category
`NSPrivacyAccessedAPICategoryUserDefaults`, reason `1C8F.1`) solely to store the
three values above and share them with its own widget extension. This is
declared in the app's bundled privacy manifest.

## Children

The app is not directed at children and collects nothing from anyone.

## Changes

Any change to this policy will be published on this page with a new date above.

## Contact

Questions about this policy: [open an issue](https://github.com/peterlvilim/endpoint-status/issues).
