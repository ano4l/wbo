WE BUILD ONCE
FINAL STANDALONE WEBSITE — CLIENT HANDOVER & PUBLISHING GUIDE
===============================================================

PACKAGE PURPOSE
---------------
This folder is the production/deployment version of the WE BUILD ONCE website.
It is intended to be uploaded to the client's web hosting account so the site can go live.

IMPORTANT: Upload the CONTENTS of this folder to the hosting account's public web directory
(commonly named public_html, www, htdocs, or public).

DO NOT upload the development project for normal website publishing.

WHAT IS INCLUDED
----------------
- index.html                 Main website entry point
- assets/                    Production CSS and JavaScript
- images/                    Website images and logos
- .htaccess                  Apache routing configuration for direct page URLs
- CLIENT_HANDOVER_README.txt This publishing and handover information

NO DEVELOPMENT PROJECT FILES ARE REQUIRED TO PUBLISH THIS VERSION.

PUBLISHING STEPS
----------------
1. Log in to the client's hosting control panel (for example cPanel).
2. Open File Manager and enter the domain's public web directory, normally public_html.
3. Upload this package ZIP.
4. Extract the ZIP in the public web directory.
5. Confirm that index.html is directly inside the public web directory.
   Example: public_html/index.html
   NOT:     public_html/WE_BUILD_ONCE_FINAL_PUBLISH_PACKAGE/index.html
6. Confirm that the assets/ and images/ folders are beside index.html.
7. Visit the client's domain in a browser.
8. Test the navigation and every main page.
9. Enable/confirm HTTPS/SSL for the domain.

MAIN WEBSITE ROUTES TO TEST
----------------------------
/
/about
/services
/leadership
/projects
/contact

If the hosting server is Apache/cPanel, the included .htaccess is intended to allow
these routes to work when visited directly.

DOMAIN & DNS
-----------
The website files do not automatically connect a domain to the hosting account.
The client's domain DNS must point to the chosen hosting provider.

The hosting provider/domain administrator should confirm:
- A/AAAA records or the provider's required DNS records are configured correctly.
- The domain resolves to the correct hosting account.
- HTTPS/SSL is active.

EMAIL
-----
The website currently displays the business contact email:
Info@webuildonce.co.za

The domain's email service is separate from the website hosting unless the hosting provider
also supplies email. Confirm that the mailbox exists and that its DNS/mail records are correct.

CONTACT FORM
------------
The current contact form prepares an email enquiry for the business rather than relying on
a custom server-side database/form-processing system.

After publishing, test the Contact page and confirm that the enquiry workflow behaves as
expected on the client's target devices/browsers.

IMPORTANT SECURITY NOTE
-----------------------
Do not add passwords, API keys, hosting credentials, database credentials, or .env files
to this website package.

FINAL CLIENT CHECKLIST
----------------------
[ ] Website files uploaded to the correct public web directory
[ ] index.html is at the web root
[ ] assets/ folder is present
[ ] images/ folder is present
[ ] HTTPS/SSL works
[ ] Home page loads
[ ] About page loads
[ ] Services page loads
[ ] Leadership page loads
[ ] Projects page loads
[ ] Contact page loads
[ ] Navigation links work
[ ] Mobile layout tested
[ ] Desktop layout tested
[ ] Contact/email workflow tested
[ ] Business email address confirmed
[ ] Domain DNS confirmed

HANDOVER NOTE
-------------
This is the production website package for publishing. Keep a separate copy of the source/
development project if future design or code changes are required. This production package
should be treated as the deployment copy.
