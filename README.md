RoboCup US @2026

Two repos hold this page, with the same content:

- `robocup-org/robocup-us-regional` publishes https://us.robocup.org with GitHub Pages, from `main`.
- `rbonill/robocup-us-regional` is a working copy with GitHub Pages turned off (2026-09-15). Changes go to the
  official repo first and are then brought into the copy.

`index.html` carries a `rel="canonical"` link to https://us.robocup.org/, so search engines treat the official page as
the original.

**us.robocupamericas.org** is not served from either repo: FastComet answers it with a 301 redirect to
https://us.robocup.org/ (folder `~/us.robocupamericas.org`, 2026-09-15).
