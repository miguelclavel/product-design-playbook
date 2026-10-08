# Launch checklist for a site

The checklist I ran my chat portfolio against, trimmed to what applies to most sites. Run it before launch, and again after any big change.

## Security
- [ ] No secrets in the code, the git history, or the published files
- [ ] Secrets live only in the host's environment settings
- [ ] Only the site itself is uploaded (no `.git`, no config files); hidden files return 404
- [ ] HTTPS everywhere, with plain HTTP redirecting
- [ ] Security headers set: Content Security Policy, HSTS, X-Frame-Options, nosniff, Referrer-Policy
- [ ] Every form and endpoint checks what it receives (type, size, where it came from)
- [ ] There's a way to roll back to the last version in one step

## Search, for Google and AI assistants
- [ ] One unique title per page, under about 60 characters
- [ ] One unique description per page, under about 160 characters
- [ ] Canonical links set; private pages marked noindex
- [ ] A share image for every important page
- [ ] Structured data for the person or organisation
- [ ] A plain text summary at `/llms.txt` for AI assistants

## Accessibility
- [ ] Contrast, keyboard paths, visible focus, alt text, reduce motion (see the [design QA checklist](design-qa-checklist.md))
- [ ] Reflows at 320 pixels wide

## Speed
- [ ] Images sized for where they're shown, and lazy loaded below the first screen
- [ ] Caching rules don't freeze old code in visitors' browsers (new code gets new file names, or short cache times)

## After launch
- [ ] Analytics working, with your own visits excluded
- [ ] A way to hear what people couldn't find or do (a log, a form, a weekly review)
- [ ] Someone owns the weekly look at it

---
From the [product design playbook](../README.md) by Miguel Clavel. MIT licensed.
