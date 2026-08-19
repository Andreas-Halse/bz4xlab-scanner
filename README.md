# bz4xlab scanner

A read-only diagnostic scanner for a 2026 Toyota bZ4X, driven from a phone over
an OBDLink CX. Sends only UDS `22` (ReadDataByIdentifier) and `3E` (TesterPresent)
requests — it contains no write, session-control, or security-access code at all.

- `index.html` — scanner, preloaded with progress from earlier runs
- `clean.html` — identical scanner with no preloaded data

Needs a browser that implements Web Bluetooth: Chrome on Android, or Bluefy /
WebBLE on iOS. Safari and Chrome on iOS cannot do it — iOS forces every browser
onto WebKit, which has no Web Bluetooth.
