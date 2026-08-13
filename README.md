# 799piedmontapartments.com

Leasing site for 799 Piedmont Ave NE, Atlanta, GA 30308 — eleven apartments in
Midtown's Garden District.

Single self-contained `index.html`, no build step. Served by GitHub Pages at
[799piedmontapartments.com](https://799piedmontapartments.com).

## Editing

| What | Where |
|---|---|
| Unit rents, sizes, availability | `UNITS[]` array near the bottom of `index.html` |
| Photo galleries | `PHOTOS{}` object, same place |
| Inquiry form destination | `access_key` hidden input in the contact form |

Availability status is one of `open`, `soon`, or `occupied`.

## Photos

Web-ready images live in `photos/`, organised by unit. Originals are kept outside
this repo and optimised with `crop-and-optimize.ps1` in the parent folder — it
strips the MLS watermark strip, corrects EXIF rotation, resizes, and re-encodes.
