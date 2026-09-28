# ARKAN COFFEE

Production domain: https://www.arkancoffee.com

This repository is connected to the existing Vercel project. Vercel forwards requests to the live ARKAN application at https://arkan-coffee-origin-gulf.melanshifa.chatgpt.site without changing the visitor's address bar.

The application serves the English and Arabic website, the protected `/admin` owner workspace, `/brand-kit`, and document exports. Its existing Cloudflare Worker and database remain authoritative. This is a routing integration, not a migration of the backend into Vercel.

Owner credentials, customer records, invoices, source workbooks and private brand files must not be committed to this public repository. Access checks stay in the application. Proxy caching is disabled to protect authenticated responses.

The application's mutation-origin allowlist includes only its own origin and the two production domains: `https://arkancoffee.com` and `https://www.arkancoffee.com`. Adding another production domain requires updating that allowlist. Untrusted cross-site mutations are rejected.

No GoDaddy DNS or email changes are required for this deployment. The prior landing page can be recovered from Git history.
