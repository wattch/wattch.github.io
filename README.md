# wattch.github.io

This [Github Pages](https://pages.github.com/) repository is used for end-to-end security testing.
It hosts static html+js pages that exercise the staging and production APIs (both the Kiosk API
and the "main" public API) to ensure that they are working.  For more info on these APIs, see:
* https://kioskdocs2.wattch.io
* https://api.wattch.io

These test pages are continuously monitored for correct behavior by our
[Betterstack](https://betterstack.com/) account.

In particular note that it is important that these test pages are NOT hosted on a wattch domain
because (due to cross-domain browser restrictions) it would be very easy to break things in such a
way that all of these test pages would still work if hosted at a wattch.io subdomain but would fail
if hosted at any other domain.
