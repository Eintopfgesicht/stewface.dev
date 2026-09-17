# EbayYearlyReport Update Authority v1

This namespace is reserved for the public update authority of EbayYearlyReport.

Planned stable endpoint:

- `https://stewface.dev/products/ebayyearlyreport/update/v1/latest.json`

Design rules:

- `stewface.dev` provides public update metadata only.
- Installer/update payloads are not stored in this Pages repository.
- Release payloads are intended to be delivered through a release host such as GitHub Releases.
- Update metadata must not contain credentials, tokens, private repository URLs, or signing private keys.
- Before activating `latest.json`, the application-side updater contract must be verified against the currently shipped parser.
- Integrity verification (at minimum SHA-256; preferably signed metadata) is required before unattended installation is enabled.

Status: infrastructure reserved; active update manifest intentionally not published yet.
