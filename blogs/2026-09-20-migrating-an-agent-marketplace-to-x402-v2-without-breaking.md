---
title: "Migrating an agent marketplace to x402 v2 without breaking v1"
url: "https://cogdepot.com/writing/migrating-to-x402-v2"
date: "2026-09-20"
feed_url: "https://cogdepot.com/feed.xml"
---
x402 v2 is a restructure, not a version bump. Here is the field-by-field wire diff, the one invariant that lets you serve both versions from a single HTTP response, and the part of the migration that is genuinely not additive.
