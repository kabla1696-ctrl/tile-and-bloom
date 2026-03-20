# CI Checklist (Game Project)

## On every PR / commit
- [ ] Build succeeds (Android dev build)
- [ ] No compile errors/warnings spike
- [ ] Basic smoke test scene runs
- [ ] Config files valid (JSON/YAML)
- [ ] No secrets committed

## Nightly checks
- [ ] Full project build
- [ ] Asset integrity check
- [ ] Crash symbol upload check (if enabled)
- [ ] Dependency drift report

## Release gate
- [ ] Release branch tagged
- [ ] Version bump verified
- [ ] Changelog/release notes updated
- [ ] QA sign-off attached
