# Data and privacy boundaries

[Overview](../README.md) · [Architecture](ARCHITECTURE.md)

Implementation summary reviewed 21 October 2026. This document explains the current prototype's data paths; it is not a security certification or a complete legal privacy policy.

## What may leave the device

| Data | Current path | User-facing implication |
| --- | --- | --- |
| Account identity | Supabase authentication. | Google sign-in authenticates identity; it does not itself connect Gmail, Google Calendar or Outlook. |
| Account plan | Supabase account snapshots for events, tasks, goals and relevant preferences. | Account mode uses cloud storage. Local mode does not provide account sync. |
| Supported Canvas feed URL | Submitted to the hosted feed endpoint to fetch a reviewed snapshot. | Treat it as a credential. The implementation does not intentionally retain the URL in saved plan records; this is not a guarantee about every infrastructure log. |
| Cloud-AI message | Request text, scope and planning date go through the server to the configured provider. | Do not type secrets or sensitive diary details. The stored calendar is not automatically attached to that request. |
| Native Apple Health readings | Read-only native connection and local summary, outside the account-plan payload. | Not automatically uploaded to account sync or cloud AI through the reviewed read path. Physical-device verification remains open. |
| Manual wellness records | Local records, with a separate optional cloud-health consent path. | These are distinct from HealthKit readings. Review the app's cloud-health setting before using this feature. |
| Optional feedback | GitHub Issues or the linked survey service when you submit. | Avoid personal calendar details. Public issues are publicly visible. |

## Controls and limits

- Imports are previewed before selection and confirmation.
- AI produces a draft; the user reviews supported changes before they are applied.
- Production cloud AI in Health mode is disabled in the reviewed code.
- Account row-level security and revision checks are implemented. They are not substitutes for hosted, multi-user isolation tests or an independent security review.
- Native title-privacy settings, quiet hours and permission controls need to be checked on the actual device/build being used.
- Missing health samples remain unknown; permission-dialogue completion does not establish permission to read every sample type.

## Reporting a problem

For routine bugs, use a sanitized [GitHub issue](https://github.com/jinghengxu74/campus-rhythm-app/issues). Do not post feed URLs, access tokens, account exports, personal health records or private screenshots.

For a suspected vulnerability, use GitHub's private vulnerability-reporting route if this repository offers it. If it is unavailable, open only a minimal request for a private contact channel, without exploit details or sensitive material. This prototype does not promise a response SLA or bug-bounty program.

## Remaining acceptance

New-user recovery, cross-device persistence, second-user isolation, physical-iPhone HealthKit authorization/read behavior and native notification privacy need continued end-to-end acceptance. No independent penetration test or compliance certification is claimed.
