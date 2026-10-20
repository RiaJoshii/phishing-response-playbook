# 01 - Scope, Roles, and Severity

## Purpose
This playbook describes how to triage and respond to reported phishing emails. It follows the NIST incident response lifecycle: preparation, detection and analysis, containment, eradication, recovery, and post-incident activity.

## Scope
This playbook covers user-reported and automatically detected phishing, including:
- **Credential harvesting links**: emails that send users to fake login pages.
- **Malicious attachments**: emails with files that run malware or exploit software.
- **Business email compromise (BEC)**: emails that impersonate executives, vendors, or coworkers to trick someone into paying money or sharing information.

## Roles
| Role | Responsibility |
|------|----------------|
| Reporting user | Reports the suspicious email and does not click, reply, or forward it. |
| Tier 1 analyst | Triages the report, checks headers, links, and attachments, and assigns an initial verdict and severity. |
| Tier 2 analyst | Performs deep analysis and carries out containment, eradication, and recovery. |
| IR lead | Takes escalations, makes decisions on high-impact incidents, and approves communications. |

## Severity Levels
| Severity | Criteria |
|----------|----------|
| **Low** | Nobody interacted with the email. |
| **Medium** | The user clicked a link, but no credentials were entered. |
| **High** | Credentials were entered, or an attachment was opened. |
| **Critical** | Confirmed compromise, or the email reached multiple users or executives. |

## Escalation
Escalate to the IR lead for any incident rated High or Critical, any email that targeted executives, or any email that reached multiple recipients.
