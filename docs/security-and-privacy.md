# Security and privacy

[← Back to the showcase](../README.md)

Masting is a supervised business email service. Security controls help define who can access company information; they do not turn the service into end-to-end encrypted personal messaging.

## Company boundaries

Company information is organization-scoped. Application access checks are backed by database-level row isolation. Company roles separate agent workflows from management operations, while platform operators have their own permissions.

## Approved networks

Authenticated access can be restricted to approved IPv4/IPv6 addresses and networks. The policy covers the workspace and its associated authenticated interfaces.

**An IP allowlist is a network boundary, not proof of physical presence.** Someone using an approved VPN exit may be outside the office.

## Supervision is intentional

Company managers can inspect their company's correspondence. Supervisory reads are audited and do not mark the message read in the agent's mailbox. Privileged platform access is also audited.

People using a company mailbox should understand their employer's supervision policy. Masting does not claim that the service operator or company management is technically unable to read mail.

## Handling untrusted email

HTML email is sanitized and displayed in a sandboxed frame without scripts. Remote images are blocked by default. Risky attachments receive protective handling.

These measures reduce exposure; they are not a guarantee that every message or attachment is safe.

## Credentials and authentication

Connection credentials stay server-side and are encrypted at rest rather than sent to browsers.

Two-factor authentication is a configurable capability. Actual enforcement depends on the deployed role policy. This showcase does not claim that MFA is currently enabled or mandatory for every role.

## Sending controls

Recipient verification and suppression rules apply to sending. Tunnel-required routes fail closed rather than silently sending directly. Delivery statuses distinguish confirmed SMTP acceptance from inbox placement, which is not guaranteed.

## Limits of the claims

This repository does not claim:

- End-to-end encryption.
- A compliance certification or independent security audit.
- An uptime SLA.
- Guaranteed inbox placement.
- Guaranteed protection from every malicious message.
- That optional AI, payment or registrar integrations are active.

Read the [public security page](https://masting.ai/security), [Privacy Policy](https://masting.ai/legal/privacy), [Acceptable Use Policy](https://masting.ai/legal/acceptable-use) and [Terms](https://masting.ai/legal/terms). For access or security questions, contact the Masting team through [Drogoz](https://t.me/drogoz).

