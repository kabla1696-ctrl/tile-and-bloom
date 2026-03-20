# Go / No-Go Scale Rules

## GO (Scale UA) if ALL true:
- D1 >= 35%
- D7 >= 10%
- Crash-free >= 98%
- ARPDAU trending up (7-day)
- CPI within target band

## NO-GO (Do Not Scale) if ANY true:
- D1 < 30%
- Crash-free < 97.5%
- ARPDAU flat/down 14 days
- Major blocker unresolved in core loop

## HOLD (Limited Scale) if:
- Retention okay but monetization weak
- Monetization okay but retention unstable
- Creative fatigue unresolved

## Scale Steps
- 10% budget increase every 3-5 days
- Stop escalation if KPI dips beyond threshold
- Rollback to previous stable spend level
