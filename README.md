# Hermosa Epoxy website

Responsive React and Vite product catalogue with WhatsApp-first enquiries.

## Run locally
1. Install Node.js 18 or newer.
2. Run npm install.
3. Run npm run dev and open the local URL.
4. Run npm run build to create the production build in dist/.

## Configure before launch
- Edit src/config.js and set WHATSAPP_NUMBER to the official business number in international digits-only format (Kenya example: 2547XXXXXXXX). The site intentionally does not invent a contact number.
- Set BUSINESS_EMAIL if email enquiries are required.
- Replace the starter catalogue in src/products.js with verified product names, images, pack sizes, specifications and current prices. Current entries are illustrative categories, not confirmed stock or product claims.
- Business location is configured as Konza City, Machakos, Kenya. Review copy, imagery, legal/privacy requirements and contact details before publishing.
- No online payment or stock-management integration is included.

## Deploy
Run npm run build. Deploy the generated dist folder to a static host supporting SPA fallback (such as Netlify or Vercel).

## WhatsApp flow
Visitors can add catalogue items to an enquiry list. The generated WhatsApp message includes selected product names and asks the team to confirm price, pack size and suitability. Until WHATSAPP_NUMBER is configured, enquiry links lead to the Contact section.
