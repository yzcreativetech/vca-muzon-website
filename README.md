# VCA Muzon Website (Production)

This repository contains the production version of the
Victory Churches of Asia - Muzon website.

Deployment target:
https://yzcreativetech.github.io/vca-muzon-website/

Production website:
https://vcamuzon.org/

This is the canonical public production identity.

## Development workflow

Changes are implemented and approved in the separate UAT repository before
promotion to this production repository. Validate the promoted files locally,
remove UAT review markers, and push approved changes to production `main`.
Confirm the GitHub Pages deployment after publication.

## Progress

- [x] About Hero Video milestone
  - Replaced the About page static hero presentation with a looping drone video.
  - Retained the existing church image as the poster and fallback.
  - Tuned responsive video framing to `62% center` on desktop, `66% center` on
    tablets and mobile devices, and `72% center` on small phones.
  - Preserved autoplay compatibility with `muted`, `playsinline`, and `loop`.
  - Preserved reduced-motion accessibility by hiding the video and displaying
    the fallback image when reduced motion is requested.
  - Removed obsolete About hero background styles, empty portrait-tablet media
    queries, and duplicate CSS declarations.

## Release notes

### UAT - About Hero Video

The About page now uses responsive drone footage in its hero area while keeping
the original church image as a reliable poster and accessibility fallback. The
associated stylesheet cleanup consolidates superseded component rules and
removes empty responsive blocks. Validation confirmed balanced CSS braces and a
clean `git diff --cached --check` result before publication.
