# Sileo demo

A userland demo of the Sileo package manager UI, running on stock iOS — no jailbreak, no exploits, no privileges.

This is a demo, not the full Sileo app. It shows the real Sileo interface with real repository data, on a phone that was never jailbroken.

## What works

- Featured page with live data from the remote Featured list
- Real repository data: Havoc and Chariz are the default sources
- Packages tab, categories, and search over real repo metadata
- News tab with bundled articles
- Tapping GET downloads a real `.deb` file to `Documents/Downloads`
- Footer shows your real iOS version

## What does not work (honest limits)

- Package installation is not available on stock iOS. Tapping GET downloads the `.deb`, it does not install it.
- Canister is a stub — it never contacts the Canister service.
- The installed-packages list is empty: nothing is actually installed by this demo.

## Install

Sideload the IPA with your own certificate (AltStore, SideStore, LiveContainer, or similar). Minimum iOS 12.0.

## Build

Built by GitHub Actions (`.github/workflows/ipa-demo.yml`) from the `demo` branch.

## Credits

Based on [Sileo](https://github.com/Sileo/Sileo) by Amy While and contributors. Demo modifications by adnan.120hz.
