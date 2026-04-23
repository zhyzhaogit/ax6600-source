# Source Repository Bootstrap

## Purpose

This repository starts as a thin shell so you can create it early and let the firmware repository point at a stable destination.

## First Follow-Up Steps

1. Create the GitHub repository.
2. Push `main`.
3. Import the chosen upstream into `main`.
4. Create:
   - `ax6600-dev`
   - `ax6600-stable`
5. Wire `ax6600-firmware/targets/ax6600/upstreams.yml` so `source-primary` points here.

## Branch Intent

- `main`: near-upstream tracking line
- `ax6600-dev`: integration and rebase work
- `ax6600-stable`: firmware-consumed validated line
