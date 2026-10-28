# 01 - Scope and Roles

## Purpose
How to triage and respond to reported phishing emails.

## Scope
This playbook covers user-reported and detected phishing, including:
- Credential harvesting links
- Malicious attachments
- BEC (business email compromise): an attacker impersonates an executive, vendor, or coworker by email to trick someone into sending money or sensitive information

**Out of scope:** spam or marketing email with no malicious intent.

## Roles
| Role | Responsibility |
|------|----------------|
| Reporting user | Reports the suspicious email and says whether they clicked, replied, or opened anything |
| Tier 1 analyst | Triage: confirms whether the email is phishing and assigns an initial severity |
| Tier 2 analyst | Deep analysis and containment (header and URL/attachment analysis, blocking, resetting credentials) |
| IR lead | Takes escalations and coordinates the response for High and Critical incidents |

## Severity Levels
| Level | Criteria | Who handles it |
|-------|----------|----------------|
| Low | Nobody interacted with the email | Tier 1 closes it |
| Medium | The user clicked, but no credentials were entered | Tier 1 triages, Tier 2 contains |
| High | Credentials were entered or an attachment was opened | Tier 2 leads, IR lead notified |
| Critical | Confirmed compromise, or the email hit multiple users or executives | IR lead takes over, Tier 2 supports |
