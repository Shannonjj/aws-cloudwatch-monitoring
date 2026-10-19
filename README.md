# AWS CloudWatch Monitoring — Billing Alarm and Dashboards

Monitoring lab from my UMGC CCA 630 coursework: cost alerting and a custom metrics dashboard in Amazon CloudWatch.

## Billing alarm — CCA630BillingAlarm
- Created a CloudWatch alarm on the **EstimatedCharges** (billing) metric
- Condition: total estimated charges **greater than or equal to $100** for 1 consecutive period of 6 hours
- Maximum metric value used as the statistic; missing data treated as missing
- Configured an alarm-state notification (SNS topic delivery, with email confirmation flow)

## Dashboard — CCA630
Built a custom dashboard with:
- **Line widget** plotting trend metrics (including an EC2 `...Called` usage metric and a Billing `...arges` metric), period set to 1 day
- **Number widget** showing per-instance / API-usage metrics for EC2 (e.g., per-instance usage values) on a 5-minute period
- Period overrides and widget layout adjusted during the build

## Skills demonstrated
- Amazon CloudWatch alarms (metrics, thresholds, periods, SNS actions)
- Custom dashboards with line and number widgets
- AWS cost monitoring fundamentals


---
*Shannon Javone Jenkins — MS in Cloud Computing Architecture, University of Maryland Global Campus (UMGC). Graduate coursework and hands-on labs.*
