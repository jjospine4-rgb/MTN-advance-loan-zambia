# MoMo Advance Loan Portal (safe starter)

## Included
- Responsive loan calculator for ZMW 1,000–10,000 and 6/12/24/48 months.
- Application form with server-side validation.
- Express backend endpoint to receive applications.
- Phone-verification endpoints intentionally disabled until an approved SMS provider is configured.
- No collection or storage of MoMo PINs or payment-gateway OTPs.

## Run locally
1. Install Node.js 18 or newer.
2. In this folder, run `npm install`.
3. Copy `.env.example` to `.env` and configure the environment.
4. Run `npm start`.
5. Open `http://localhost:3000`.

## Before production
- Confirm you are authorized to offer loans and use any MTN/MoMo branding.
- Replace in-memory application storage with a secure database.
- Add authentication/authorization for staff, CSRF protections where relevant, data encryption, audit logging, backups, deletion/retention policy, privacy notice, and appropriate consent.
- Integrate only an approved SMS provider for verifying the applicant's own phone number.
- Use MTN's official developer/merchant onboarding and a provider-hosted payment authorization flow. Never collect MoMo PINs or gateway OTPs on this site.
- Have a qualified professional review lending disclosures, rates, fees, eligibility and local legal requirements.

The displayed monthly estimate is principal divided by term only. It is not a loan quote and excludes interest and fees. This starter does not approve or disburse loans.
