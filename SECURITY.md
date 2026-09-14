# Security

This action runs inside customers' CI with `permissions: id-token: write` and mints an OIDC token
that authorises publishing content. Please treat vulnerabilities in it accordingly.

## Reporting

Report privately through GitHub's **Report a vulnerability** button on this repository's
Security tab, or email support@leed.ai. Please do not open a public issue.

## Pinning

`@v1` is a moving tag that tracks the latest `v1.x.y` release. If your organisation requires it,
pin to a full commit SHA instead and update deliberately:

```yaml
- uses: Leed-AI/schedule-release@<full-40-character-sha>
```
