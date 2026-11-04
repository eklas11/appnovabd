APP NOVA BD — WEBSITE & SEO DEPLOYMENT GUIDE

Website: https://appnovabd.onrender.com/ Repository:
https://github.com/eklas11/appnovabd

ABOUT

App Nova BD is a web project maintained by eklas11. This repository
contains the website homepage and supporting files for search-engine
discovery, browser compatibility, and deployment.

PROJECT FILES

index.html Main homepage. Keep this filename if your hosting provider
serves index.html as the default page.

robots.txt Provides crawler guidance and points search engines to the
sitemap. Check that the sitemap URL matches the live production domain.

sitemap.xml Lists URLs that may be discovered by search engines. Keep it
accurate and include only canonical, publicly accessible pages.

site.webmanifest Web-app metadata used by supported browsers when the
site is installed.

browserconfig.xml Legacy Windows tile configuration.

favicon.png Website icon. Confirm that this file exists at the deployed
site root and that the homepage references the correct path.

404.html Custom not-found page for hosting platforms that support this
file.

_redirects Redirect rules for hosts that support the Netlify _redirects
format. This file is not automatically supported by every hosting
provider.

_headers HTTP header rules for hosts that support the Netlify _headers
format. Configure equivalent headers separately if your host does not
support it.

humans.txt Optional project and site credits.

security.txt Security contact template. Replace any placeholder contact
information with a monitored address before publishing.

SEO-CHECKLIST.txt Checklist for reviewing search-engine setup.

Google verification HTML file Used for Google Search Console ownership
verification. Keep the exact filename provided by Google and place it at
the website root.

DEPLOYMENT CHECKLIST

1.  Upload the website files to the correct repository or deployment
    folder.
2.  Confirm that index.html is at the published site root.
3.  Open the live homepage and check that it loads correctly on mobile.
4.  Check these URLs in a browser:
    https://appnovabd.onrender.com/robots.txt
    https://appnovabd.onrender.com/sitemap.xml
    https://appnovabd.onrender.com/site.webmanifest
5.  Confirm that every URL listed in sitemap.xml is a real, canonical
    page.
6.  Verify the site in Google Search Console.
7.  Submit the sitemap.xml URL in Search Console.
8.  Inspect the homepage URL and review any indexing errors.
9.  Test all navigation links, images, favicon, and the 404 page.
10. If using Render, confirm which routing and header features Render
    supports. Do not assume _redirects or _headers are applied
    automatically.

SEO NOTES

-   These files help with technical setup; they do not guarantee
    rankings.
-   Search engines decide when and whether to crawl, index, and rank
    pages.
-   Useful original content, clear page titles, descriptive meta
    descriptions, mobile usability, performance, internal links, and
    trustworthy references also matter.
-   Keep the sitemap and canonical URLs consistent with the actual live
    domain.
-   Do not add pages to the sitemap that return errors, redirect
    elsewhere, or are marked noindex.
-   Avoid keyword stuffing, hidden text, copied content, and misleading
    metadata.
-   Recheck Search Console after major website changes.

MAINTENANCE

Update the documentation whenever the domain, hosting provider, file
paths, or deployment process changes. Never publish passwords, private
API keys, access tokens, or other confidential credentials in this
repository.

PROJECT OWNER

GitHub account: eklas11 Project: App Nova BD

This README describes the repository files and suggested deployment
checks. It is not a guarantee of search-engine indexing, traffic, or
ranking.
