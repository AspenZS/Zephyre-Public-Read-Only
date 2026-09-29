# Live Zephyre Systems public status

Use the canonical Zephyre endpoint for current status. The server reads the published Uptime Kuma sources for every request, returns `Cache-Control: no-store`, and includes a `generatedAt` timestamp in the response.

- [Fetch live canonical status JSON](https://zephyresystems.com/status.json?via=github)
- [Fetch live canonical status as readable text](https://zephyresystems.com/status.md?via=github)
- [Independent freshness check](https://zephyresystems.com/status.json?via=github-freshness-check)

The second link reaches the same read-only handler through a distinct request URL so an assistant can verify that a later query has a newer `generatedAt` timestamp.

The files `status.json` and `status.md` in this repository are hourly fallback snapshots only.
