# AB Explainer Updates

Signed and notarized macOS releases for AB Explainer.

- [Download the latest release](https://github.com/Asianboss-AI/ABExplainer-Releases/releases/latest)
- [Sparkle update feed](https://asianboss-ai.github.io/ABExplainer-Releases/appcast.xml)

The application source is maintained privately. This repository contains only public update metadata and release assets.

## Current release

[**AB Explainer 1.0.0 (19)**](https://github.com/Asianboss-AI/ABExplainer-Releases/releases/tag/abexplainer-v1.0.0-b19) adds direct caption editing and Enter line breaks. Manual edits stay out of AI feedback and company examples.

The release ZIP is signed and notarized. SHA-256: `51d655f0d7bbba5ee682b7f7189f4795c2481f60cdbcb113e48899884bc2410b`.

## Publishing updates

1. Build a new release with an increasing bundle build number and the existing production Sparkle public key.
2. Verify Developer ID signatures, Apple notarization, stapling, Gatekeeper, and the extracted ZIP.
3. Generate and verify the archive signature and signed appcast with the matching production key.
4. Publish the ZIP as a release asset, download it without authentication, and verify its size and SHA-256 against the local file.
5. Commit the signed `appcast.xml` last, then verify the live Pages feed and its signatures.

Do not edit a signed appcast without signing it again. Private keys, credentials, and application source do not belong in this repository.

## Recovery baseline

The update feed was restored on 2026-10-15 using the previously distributed **1.0.0 (18)** release. Its ZIP SHA-256 is `67549621e4809ceecdf4ff895ecf2c974062ba74fe3e714a2cafff3c64495d0f`.
