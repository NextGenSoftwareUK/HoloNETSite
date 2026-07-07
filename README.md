# HoloNET

**The World's First .NET & Unity Client for Holochain**

HoloNET is an open-source library that allows any .NET application, Unity game or Unreal Engine project to connect to the [Holochain](https://holochain.org) peer-to-peer network. It is the foundational bridge between the Microsoft ecosystem and Holochain's agent-centric distributed computing framework — and a core piece of the OASIS Omniverse technical stack.

## Components

| Component | Description |
|---|---|
| **HoloNET Client** | Core WebSocket client for .NET ↔ Holochain conductor communication |
| **HoloNET ORM** | Object-Relational Mapper for automatic .NET object ↔ Holochain entry mapping |
| **HoloNET Manager** | GUI management tool for Holochain conductors, cells and zomes |
| **HoloNET HDK** | Holochain Development Kit extensions for .NET |
| **HyperNET** | High-level abstraction layer unifying HoloNET with the OASIS API |

## Key Features

- Full async/await support with cancellation tokens
- Automatic serialization/deserialization of .NET objects to Holochain entries
- Support for Unity and Unreal game engines (including WebGL builds)
- Integrated logging and error handling via NextGenSoftware.Logging
- Used internally by the OASIS API as one of its 40+ provider implementations

## Use in the OASIS Omniverse

HoloNET powers the Holochain storage provider within the OASIS API, enabling:
- Decentralized avatar data storage
- Peer-to-peer karma ledger
- Distributed NFT and asset management
- P2P quest and mission state

## Related Repositories

- [`OASIS2`](../OASIS2) — the main OASIS API and platform
- [`OASIS-Holochain-hApp`](../OASIS-Holochain-hApp) — the Holochain hApp that HoloNET connects to

## Tech Stack

This repo contains the **landing page site** for HoloNET (`index.html`). The actual HoloNET library source lives in the `OASIS2` monorepo.

| Layer | Detail |
|---|---|
| Site | Single-file `index.html` — inline CSS + vanilla JS |
| Fonts | Orbitron, Rajdhani, Share Tech Mono (Google Fonts) |

## Running the Site Locally

```bash
npx serve .
# or
python -m http.server 8080
```

---

*Part of the [OASIS Omniverse](https://oasisomniverse.one) · Built on [Holochain](https://holochain.org)*
