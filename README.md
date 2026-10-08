# Hero Cycles – Government Supply Monitoring Portal (Demo)

A front-end demo of a web portal that gives Hero Cycles end-to-end visibility of bicycle supply to Government institutions: from tender planning and factory production, through QR-tracked dispatch, site unloading, fitting and school delivery, to invoicing and payment collection.

**Live demo:** https://&lt;your-username&gt;.github.io/hero-cycles-portal/

## Sign in

1. Pick a persona on the sign-in page (Super Admin, Admin, Factory, Transporter, Site Supervisor, Government Official or Finance).
2. Enter OTP **123456**.
3. If a second code is requested (Admin, Finance, Super Admin), press **Autofill** or enter any 6 digits.

Each persona sees only the modules and States its role allows. To try another role, sign out and sign in again.

## What the demo covers

| # | Module | What you can see |
|---|---|---|
| 1 | Pre-tender planning | Government departments, anticipated tender month and quantity |
| 2 | Supply orders | PO, rates, district / school allocation, document repository |
| 3 | Production & QR | QR codes for every frame and accessory package, label preview, QR trace lookup |
| 4 | Transport & GPS | Transporter, vehicle and driver details, shipment QR, live fleet map |
| 5–6 | Scan monitor | Loading and unloading scans from the companion app, loaded vs unloaded reconciliation, shortages |
| 7 | Bicycle fitting | Fitter OTP attendance, live fitting counts, supervisor approval, productivity |
| 8 | Quality inspection | Inspection, lab and third-party reports |
| 9 | Delivery & challans | Delivery challan generation, signed copy, Government verification |
| 10 | Payment monitoring | Invoiceable quantity, GST, finance approval, 30/60/90/120-day ageing, UTR reconciliation |
| 11 | Service camps | Camp schedule, attendance and photos |

Also included: command dashboard with exceptions, alerts and notifications, MIS reports with Excel / PDF export, role-based and State-wise access, and an audit trail.

## Key assumptions

- **All QR scanning happens in the Android companion app.** The portal does not scan; it plans, approves, monitors and invoices. App scans are simulated and arrive every few seconds.
- **The portal's QR code engine generates the codes.** If key cycle components already carry QR codes from the factory or SAP, the same engine would register those codes instead.
- **SAP S/4HANA remains the ERP of record** for orders, deliveries, billing and payments.

## About this demo

- Front end only. All data is illustrative sample data held in the browser and resets on page reload. Names, orders and amounts are not real.
- Built with React 18, TypeScript, Tailwind CSS and Vite, plus Leaflet / OpenStreetMap for maps and jsPDF / SheetJS for exports.
- This repository contains the built static site, served with GitHub Pages.
- The back-end implementation and integration approach is described in a separate document.

Hero Cycles name and logo belong to Hero Cycles Ltd. and are used here only to illustrate the proposal.
