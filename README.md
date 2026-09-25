# WE BUILD ONCE

Standalone production website export for Vercel.

## Deploy on Vercel

This is a static SPA export. Import the repository into Vercel with the project root set to the repository root. No build command, output directory, framework preset, or environment variables are required.

`vercel.json` maps the client-side routes back to `index.html`, so direct visits and refreshes work for the main pages.

## Local preview

Serve this directory with any static web server, for example:

```powershell
python -m http.server 4173
```

Then open `http://localhost:4173`.

## Contact form

The enquiry form opens the visitor's default email application and prepares a message addressed to `Info@webuildonce.co.za`. It does not require a server-side API or credentials.
