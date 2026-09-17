# Shopify App — Project Handoff

Written 2026-09-17 at the end of the planning session that chose this direction.
Read fully before doing anything; it replaces re-deriving the context.

## Who and why

- Owner: Shakil (schackeel@gmail.com), Bahrain. Expat on a sponsored work visa.
- Employed full-time at Almoayyed International Group — Microsoft Dynamics 365 /
  Business Central / Power Platform / SharePoint implementation work.
- Goal: a solid, safe side income. Effort is NOT the constraint — a second team
  member can be added. Safety from employment conflict IS the constraint.
- Platform decision: Shopify app (chosen over WordPress plugin, micro-SaaS, mobile
  app). Reasons: merchants are businesses and pay monthly; Shopify Billing charges
  0% on the first $1M/yr (verify current terms); App Store distribution; Node/React
  skills already exist; payout is royalty-shaped, which keeps the visa question narrow.

## Hard constraints — do not violate

1. NO overlap with the employer's field: nothing touching Microsoft Dynamics,
   Business Central, Power Platform, AppSource, or ERP integration to those systems.
   Accounting sync to Zoho Books / Xero / QuickBooks is fine; to Business Central is not.
2. NO employer inputs: no client data, code, documents, methodology, working hours.
   The planning laptop was domain-joined (Almoayyedintl.com). Build on personal
   hardware, personal connection, personal accounts. Rebuild rather than copy.
3. Legal position must be verified before revenue: (a) visa permission to receive
   international royalty income via a third-party platform; (b) employment contract
   clauses — exclusivity, moonlighting, IP assignment, non-compete; (c) written
   approval if the contract requires it. Ask the narrow question ("royalty income
   from software sold internationally through a platform"), not "may I run a business".
4. Verify Shopify Partner payout methods available in Bahrain BEFORE building.
   PayPal receiving/withdrawal has been limited there. If you can't get paid, stop.

## Niche direction (chosen, not yet validated)

GCC compliance and operations — legally required or operationally necessary,
regionally specific, outside the checkout critical path (so an outage is an
inconvenience, not lost sales — important for a part-time team).

Candidates, in priority order:
1. KSA ZATCA e-invoicing for Shopify merchants (structured, signed e-invoices,
   phased mandate). Lexware/Revoq-shaped niche: legally required, regional, few
   global competitors. NOTE: Microsoft partners also implement ZATCA inside
   Business Central for enterprise clients — a Shopify app for small merchants is a
   different product for a different customer, but name it explicitly in any
   employer approval conversation.
2. GCC VAT-compliant invoices (Bahrain, UAE, KSA, Oman — tax-authority-correct).
3. COD operations for the Gulf: forms, OTP, local couriers (Aramex, SMSA), Arabic RTL.
   Releasit (2,515 reviews) proves the demand globally.
4. Accounting sync to Zoho Books / Xero / QuickBooks for GCC merchants.
5. Arabic-first storefront tooling (RTL options, swatches, size charts).

Market evidence gathered from the App Store (2026-09-17, review counts as demand
proxy; installs run ~20-50x reviews): Subscriptions (Appstle 8,734), Product options
(Globo 5,034), Loyalty (Smile 4,588), Tracking (17TRACK 4,351), Upsell (~2,700 each),
Invoices (Order Printer Pro 2,901), COD forms (Releasit 2,515), EU withdrawal button
(Revoq 546), German accounting sync (Lexware 279). Top categories are owned by
5-star incumbents with free plans; the openings are regional/legal niches.

## Immediate next steps

1. Validate the niche: search the App Store for ZATCA / e-invoice / VAT invoice /
   COD apps targeting KSA/GCC. Record each one's reviews, rating, pricing, last
   update, and what one-star reviews complain about. Decide if the gap is real.
2. Check Shopify Partner payout availability for Bahrain and current revenue-share
   terms (developer docs + Partner dashboard).
3. Create a Shopify Partner account and a development store.
4. Scaffold with Shopify CLI (Remix template), Polaris, GraphQL Admin API.
5. Write a one-page MVP spec: the single legal requirement done perfectly,
   free trial + one paid plan via Billing API, GDPR webhooks, privacy policy.
6. Plan hosting (Fly.io / Railway / small VPS) with uptime monitoring.

## Reference

- Planning runbook (P-1 legal checklist, tickable):
  https://claude.ai/artifact/4XZDcuiKoMZ47Ww6YnHooh
- Prior assets on this machine (do not copy to the new product; provenance):
  D:\Shakil\Swapt (React Native + NestJS skill-exchange app, parked as portfolio)
  D:\Shakil\wp-site (local WordPress + WP Tools plugin, 31 browser tools)
