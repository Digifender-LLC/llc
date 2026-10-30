# Digifender bookkeeping procedure

**Status:** Idaho LLC approved 30 October 2026 (file # 7029055, filing date 1 October 2026). Stripe Treasury was selected as the planned financial account, and the EIN was issued 30 October 2026 (kept privately), but no opened account has been documented in this folder. This is a working record system, not a filed tax return.

## Low cost setup

Use the local `Digifender Bookkeeping.xlsx` register and original source files in the year folders. No bookkeeping subscription is needed at the current expected scale. The workbook is an internal cash activity log and review aid; its operating result is **not** automatically taxable income. Keep the business's transactions separate from household spending once the entity is accepted and an account is available. If an owner pays a setup cost personally, record it on the `Setup spend` sheet with the receipt; decide later whether it is reimbursed or contributed and how it is classified for tax.

Do not put SSNs, full card numbers, bank passwords, or account credentials in the workbook or send them in chat. Keep original invoices, receipts, bank statements, and payment processor reports, not just the spreadsheet entry. The IRS calls for records that support gross receipts and expenses and can be reconciled to the books and return. [IRS Publication 583](https://www.irs.gov/publications/p583)

## What to save each month

1. Export the Stripe Treasury financial-account statement as PDF and transaction report as CSV when available. Put the originals in `2026/Bank Statements/` (or the matching later year).
2. Export the payment processor's sales, refund, fee, tax, and payout reports. Put the originals in `2026/Processor Reports/`.
3. Save invoices and expense receipts in `2026/Receipts/`. Give each a stable filename such as `2026-10-15_vendor_amount_invoice.pdf`.
4. Save customer location and product or service type in the source sales report. This supports later state tax review; the bookkeeping register does not decide which sales are taxable.
5. If the owners paid a business cost personally, add it to `Setup spend` with payer, amount, purpose, and receipt path.

## How to record transactions

- Use one row per economic event in `Transactions`. Record **gross customer payments** as revenue, refunds separately, and payment processor fees as operating expense. A processor payout moved to the bank is a transfer, not a second sale. This keeps the books reconcilable to processor records and any Form 1099-K. [IRS Form 1099-K guidance](https://www.irs.gov/businesses/what-to-do-with-form-1099-k)
- Record owner cash added as `Member contribution`, and cash taken out as `Member distribution`. Neither is a sale or ordinary operating expense. Enter which owner was involved. Preserve these records for the partnership's capital reporting. [IRS Form 1065 instructions](https://www.irs.gov/instructions/i1065)
- Record sales tax collected separately from revenue and remitted separately from operating expense. Have the actual product and customer states reviewed before charging tax; SaaS and AI offerings can have different rules across states.
- Mark ambiguous items `Other review`; do not guess a tax deduction. The workbook's `Operating result` excludes setup spend, assets, owner funding, loans, transfers, and tax collections.

## Monthly close with Codex

Give Codex the new statements, processor reports, receipts, and the current workbook. Ask it to import or enter the transactions, match each bank and processor line once, attach evidence paths, flag missing receipts and unclear classifications, reconcile beginning plus cash in minus cash out to each ending statement balance, and provide a short exception list. Ender resolves or delegates unclear items and signs off on each month before it is marked closed. Codex can review files placed here during an active task; it cannot see new bank activity or monitor an account on its own without a separate connection or future uploads.

At year end, preserve the closed workbook and statements. If the two-member LLC uses partnership taxation and has income or deductible/creditable expenditures, Form 1065 and two Schedules K-1 will generally need preparation. A domestic partnership with neither income nor such expenditures may be excepted, so determine the requirement from the actual year, not projected profit. [IRS Form 1065 instructions](https://www.irs.gov/instructions/i1065)

## Next formation steps

- Done: filing receipt, accepted certificate, and formation date saved in `01 Formation/Idaho/`.
- Done: EIN issued 30 October 2026. Resolve the IRS single-member classification versus the planned partnership treatment before the first return (see `00 Start Here/README.md`).
- Open the selected Stripe Treasury business financial account after the EIN is available, and save its governing account agreement. Record opening deposits by owner. Decide the Stripe customer payment and billing setup before first paid sales.
- Finish and sign the 50/50 operating agreement, including contributions, distributions, authority, and deadlock rules, before substantial activity.
- Before first paid sales, review sales tax treatment for the specific SaaS/AI products and customer states. Before working from South Korea, confirm any applicable USFK/SOFA and host-country work rules.

**When to upgrade the tools:** Reassess the spreadsheet if transactions become numerous, recurring subscriptions or deferred revenue become complex, payroll begins, or a tax preparer needs a formal general ledger. Continue to keep exports and original source documents even if software changes.
