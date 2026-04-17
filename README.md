# uiao-gos — dissolved into WhalerMike/uiao

> **This repository has been dissolved.** `uiao-gos` was never a
> firewalled commercial product; the federal/commercial firewall
> doctrine was retired by
> [ADR-028](https://github.com/WhalerMike/uiao/blob/main/core/canon/adr/adr-028-monorepo-consolidation-gos-integration.md)
> on 2026-04-17. The directory-migration work that lived here is
> now part of the consolidated substrate at
> [`WhalerMike/uiao`](https://github.com/WhalerMike/uiao).
>
> Full history was preserved via `git subtree`. No content was lost —
> it was redistributed to its canonical home.

## Where everything went

| What was in `uiao-gos` | Where it lives now |
|---|---|
| BlueCat Address Manager adapter | Registry entry `bluecat-address-manager` in [`uiao/core/canon/modernization-registry.yaml`](https://github.com/WhalerMike/uiao/blob/main/core/canon/modernization-registry.yaml); implementation scaffold at [`uiao/impl/src/uiao_impl/adapters/ipam/bluecat/`](https://github.com/WhalerMike/uiao/tree/main/impl/src/uiao_impl/adapters/ipam/bluecat) |
| Infoblox NIOS adapter | Registry entry `infoblox-nios` in [`uiao/core/canon/modernization-registry.yaml`](https://github.com/WhalerMike/uiao/blob/main/core/canon/modernization-registry.yaml); implementation scaffold at [`uiao/impl/src/uiao_impl/adapters/ipam/infoblox/`](https://github.com/WhalerMike/uiao/tree/main/impl/src/uiao_impl/adapters/ipam/infoblox) |
| Directory-migration narrative | [`uiao/docs/narrative/governance-os-directory-migration.md`](https://github.com/WhalerMike/uiao/blob/main/docs/narrative/governance-os-directory-migration.md) |
| Address governance comic | [`uiao/docs/publications/series-assets/UIAO-Address-Governance-Flow.jpg`](https://github.com/WhalerMike/uiao/blob/main/docs/publications/series-assets/UIAO-Address-Governance-Flow.jpg) |
| Five-phase modernization model | Folded into ADR-028 and [`uiao/core/canon/modernization-registry.yaml`](https://github.com/WhalerMike/uiao/blob/main/core/canon/modernization-registry.yaml) |
| Roadmap adapters (users, GPOs, DNS, DHCP, PKI, RADIUS, Kerberos) | Future-work items in [`uiao/core/canon/modernization-registry.yaml`](https://github.com/WhalerMike/uiao/blob/main/core/canon/modernization-registry.yaml); not yet implemented |

## Why dissolved

`uiao-gos` was originally scoped as a firewalled commercial module
outside the federal substrate. That doctrine did not survive
contact with the actual adapter taxonomy: every adapter in `uiao-gos`
is a **modernization adapter** with `class: modernization` and
`mission-class: integration`, which is exactly the slot already
defined in
[`modernization-registry.yaml`](https://github.com/WhalerMike/uiao/blob/main/core/canon/modernization-registry.yaml).
ADR-028 retired the firewall and folded the content into the
consolidated substrate.

## This repo is now read-only

No new commits will land here. File issues and open PRs against
[`WhalerMike/uiao`](https://github.com/WhalerMike/uiao).
