# sleevenotes.ink

The public face of Sleevenotes: a landing page, the privacy policy Apple requires
before external TestFlight testing, and the share page that renders a shared card.

Static files, no build step. GitHub Pages serves this repo at `sleevenotes.ink`.

    /                 landing page
    /privacy/         privacy policy — the URL given to App Store Connect
    /s/               share page; cards arrive in the URL fragment
    style.css         one stylesheet for all of it
    CNAME             the custom domain Pages binds to

The app builds share links as `https://sleevenotes.ink/s/#...`. Everything about a
shared card rides in the fragment, which browsers never send to a server, so no web
log here or anywhere else records what was shared.
