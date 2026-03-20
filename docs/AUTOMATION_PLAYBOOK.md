# Automation Playbook

## Daily Automations
1. Pull latest analytics data snapshot
2. Generate KPI summary (DAU, Revenue, D1, Crash)
3. Flag anomalies based on thresholds
4. Post daily summary in team channel/doc

## Weekly Automations
1. Export experiment results
2. Rank levels by fail rate
3. Rank ad placements by ARPDAU impact
4. Prepare weekly scorecard draft

## Suggested Tooling
- Cron + shell/python scripts
- Firebase export jobs
- Sheets/Looker dashboard refresh
- GitHub Actions for docs consistency checks

## Automation Rules
- Never auto-deploy monetization changes without review
- Auto-alert only on meaningful threshold breaches
- Keep logs for every automated report
