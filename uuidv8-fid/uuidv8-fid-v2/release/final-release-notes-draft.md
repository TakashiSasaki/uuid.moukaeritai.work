# Final Release Notes Draft

This document is strictly non-normative.
This is a draft for future release notes and does not by itself create a Git tag or GitHub Release.

## Overview
The UUIDv8-FID-v2 specification establishes a registry and robust validation framework for stable, distributed uniqueness identifiers.
It uses a split-canonical publication model, where the split Markdown files in `uuidv8-fid/uuidv8-fid-v2/` remain the canonical source and only maintained publication form. Generated single-file Markdown output is on-demand only and not committed.

## Format ID Registry Summary
* Assigned Format ID: `0x10 time48-rand`.
* Reserved ranges: `0x00..0x0f` and `0xf0..0xff`.
* Unassigned extraction/conformance example: `0x7a` remains unassigned.

## Tooling and Support
* Validation and conformance material are included as Markdown test vectors and structural JSON vectors.
* Implementation pseudocode and tooling support correct implementations without introducing normative deviations.
