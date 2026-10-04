# Digifender business software plan

**Working plan, 1 October 2026.** Idaho formation is pending. This records software choices and launch checks; it does not open accounts or activate Whumpo billing. Recheck vendor terms and prices before subscribing.

## Use the stack already chosen

| Need | Current approach | Next check |
| --- | --- | --- |
| Customer billing | Stripe Payments/Billing work in Whumpo's sandbox. Paid subscriptions are not live. | Complete the product, tax, refund, cancellation, webhook and entitlement acceptance before live charges. See [Whumpo payment status](../../Whumpo/docs/payments.md). |
| Business funds | Stripe Treasury is the selected account, but opening is not documented. | Open after formation and EIN; verify both members' access and Ender's approval controls against the actual account features. See [banking decision](../04%20Finance/Business%20Banking%20Comparison.md). |
| Bookkeeping | [Local workbook](../04%20Finance/Digifender%20Bookkeeping.xlsx), source statements and receipts, monthly reconciliation with Codex, Ender's signoff. | No accounting subscription at the expected initial volume. Reassess if transactions, deferred revenue, payroll, or preparer needs outgrow the register. See [procedure](../04%20Finance/Bookkeeping%20Procedure.md). |
| Product operations | Whumpo's Cloudflare deployment and existing operational tools. Adminifender is under development. | Keep human review and provider dashboards as the authority until Adminifender integrations are deployed and tested. See [Adminifender status](../../Adminifender/README.md). |

## Set up or verify next

1. **Company mail.** Confirm `legal@digifender.com` can receive, send/reply, preserve messages, and be monitored by both owners with multifactor authentication and absence coverage. Add `support@digifender.com` as an alias or shared inbox when customer support opens. If an existing mailbox already does this, buy nothing. Cloudflare Email Routing can forward incoming mail to an existing inbox; a suitable mail provider is still needed for ordinary two-way correspondence. [Cloudflare email records](https://developers.cloudflare.com/dns/manage-dns-records/how-to/email-records/) · [Whumpo legal adoption checklist](../../Whumpo/docs/legal/adoption-checklist.md)
2. **Credential vault and MFA.** Use separate owner logins for Stripe, Cloudflare, GitHub, the domain registrar and the mailbox where supported. Store recovery codes securely; share only company-owned credentials through a vault, not the bookkeeping workbook or chat. If the owners do not already have a shared vault, [Bitwarden's free two-person organization](https://bitwarden.com/help/getting-started-organizations/) is a possible zero-subscription starting point. Confirm its current limits before adopting it.
3. **Alerts and restore practice.** Send available Cloudflare and Stripe account/security/failed-payment alerts to a monitored company inbox. [Cloudflare email notifications](https://developers.cloudflare.com/notifications/) are available on Free plans, but individual alert types and health checks may require higher plans. Do not assume a dashboard status is an alert. Before customer data is entrusted to Whumpo, verify a complete backup and restore path using its actual production data; the [Whumpo acceptance record](../../Whumpo/docs/acceptance.md) still leaves whole-app recovery open.
4. **Product email delivery.** When Whumpo needs to send account, billing, or customer-site notifications, select a transactional delivery service and verify sender DNS, retries, bounces, and cost. This is separate from the owners' correspondence mailbox. The [Whumpo backlog](../../Whumpo/docs/roadmap/backlog.md) still lists provider selection for contact notifications. [Cloudflare Email Service](https://developers.cloudflare.com/email-service/) currently distinguishes free inbound routing from its outbound sending beta on Workers Paid; review the actual entitlement before enabling it.
5. **Calendar.** Put Idaho annual report, registered-agent renewal, domain renewal, tax preparation, and any required copyright-agent renewal dates in the owners' existing calendar. A new project-management app is unnecessary for two owners. Confirm exact deadlines from issued records and official notices.

## Defer subscriptions until there is a reason

- **QuickBooks or another general ledger:** consider when the workbook stops reconciling cleanly, customer billing becomes complex, or the tax preparer requires a formal ledger.
- **Helpdesk/CRM:** start with the monitored support mailbox and a simple issue log. Revisit when requests cannot be tracked and answered reliably.
- **Payroll/HR:** no first-year employees are expected. Member distributions are not payroll.
- **Separate analytics, automation, or AI finance tools:** use the product and provider reports already available. Add software only for a measured gap, with approved access and data handling.

**Tax preparation is a service decision, not a standing software subscription.** A two-member LLC taxed as a partnership generally reports through Form 1065 and partner Schedules K-1 when it has reportable activity. Confirm filing requirements from the actual tax year; the overseas move and member capital/IP contributions make early preparer review worthwhile. [IRS Form 1065](https://www.irs.gov/forms-pubs/about-form-1065) · [existing bookkeeping procedure](../04%20Finance/Bookkeeping%20Procedure.md)
