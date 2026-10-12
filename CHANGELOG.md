# Changelog

## v1.0.1

- Renamed the action to "Leed - Continuous Documentation Release" and described it as continuous documentation for Leed, so it can be found by those terms in GitHub Marketplace. No change in behaviour.

## v1.0.0

First release.

- Schedules every Leed page tagged with a commit from the release to publish at one time,
  authenticating with a GitHub OIDC token.
- Works out the release without configuration: the previous matching tag on a tag build, the ref's
  previous value on a branch push, or a merge commit's parents when there is no previous value.
- `source-ids` accepts an explicit list instead of a commit range.
- Always performs a dry run first, drains past Leed's per-call page limit, and fails the job on any
  per-page failure.
