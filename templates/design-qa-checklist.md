# Design QA checklist

Run it on the real build, not the design file, before anything ships.

## Every state
- [ ] Empty, loading, error and success states exist and say something useful
- [ ] Error messages say what happened and what to do next, in plain words
- [ ] Long names, long numbers and missing data don't break the layout
- [ ] Confirmations are honest (a mail link says "your email app should open", not "sent")

## Every size
- [ ] Works on a phone, a tablet and a wide screen
- [ ] Reflows at 320 pixels wide without horizontal scrolling
- [ ] Touch targets are big enough to hit with a thumb

## Every input
- [ ] Every action works with a keyboard alone, in a sensible order
- [ ] Focus is always visible
- [ ] Menus open, move with the arrow keys, and close with Escape
- [ ] Forms label every field and announce errors

## Seeing it
- [ ] Text contrast passes WCAG AA in light and dark mode
- [ ] Nothing important is carried by colour alone
- [ ] Images have useful alt text, or empty alt text when they're decoration
- [ ] Motion respects "reduce motion"

## Measuring it
- [ ] Every link and button has a clear name in analytics
- [ ] Nothing private (what people type, emails, IP addresses) is sent to analytics

---
From the [product design playbook](../README.md) by Miguel Clavel. MIT licensed.
