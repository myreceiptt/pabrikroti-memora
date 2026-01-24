# PABRIK ROTI

[![version](https://img.shields.io/badge/version-2.4.74-blue)](https://github.com/myreceiptt/pabrikroti-master/releases/tag/v.2.4.74-inamotion) _Latest Release_  
[![status](https://img.shields.io/badge/status-active-brightgreen)](https://github.com/myreceiptt/pabrikroti-master/blob/preview/SECURITY.md#-supported-versions) _Maintenance Status_  
[![Build Status](https://github.com/myreceiptt/pabrikroti-master/actions/workflows/ci.yml/badge.svg)](https://github.com/myreceiptt/pabrikroti-master/actions/workflows/ci.yml) _CI Status_  
[![Deployed to Vercel](https://img.shields.io/badge/Vercel-deployed-success?logo=vercel)](https://preroti.endhonesa.com/) _Staging Site_

> "This is not just a factory. This is a rehearsal of freedom—kneaded with code, fermented by its community, and baked through the heat of shared struggles."
>
> — Prof. NOTA

## 📚 Table of Contents

- [Quick Start](#-quick-start)
- [Licensing & Usage](#-licensing--usage)
- [Manifestos](#-manifestos)
- [Getting Started](#%EF%B8%8F-getting-started)
- [Resources](#-resources)
- [Contributing](#-contributing)

---

## 📦 Staging 2.4.74 by Ina Motion

Link #1: [memora.voyage.co.id](https://memora.voyage.co.id/) [![status](https://img.shields.io/badge/deploy-live-brightgreen)](https://memora.voyage.co.id/)  
Link #2: [memora.endhonesa.com](https://memora.endhonesa.com/) [![status](https://img.shields.io/badge/deploy-live-brightgreen)](https://memora.endhonesa.com/)

---

## 🚀 Quick Start

```bash
yarn install && yarn dev
```

> If you find this useful, consider starring ⭐ the repository! Please!
>
> — Prof. NOTA

---

## About This Repo

This repo is a **MeMoRa** staging build for **Voyage.Co.Id**: a Web3-ready web app for commemorating experiences with **virtual collectibles** and gated media/content. It is built as a production-safe artefact that combines storytelling, collectibles, and optional access control through onchain identity.

### What it does

- Runs a multi-mode site (domain-based) that can render a full landing experience or a logged-in/gated experience.
- Provides collectible flows for **NFTs** and supporting utilities for **FTs**:
  - NFTs: `/free`, `/paid`, `/token/[idNFT]`
  - FTs: `/coins`, `/address/[coinAddress]`
- Includes content surfaces beyond collectibles (e.g. curated pages, “perks”, and media playback), including an **HLS playlist API** (`/api/playlist`) used by media pages.

### Blockchain & onboarding

- This deployment is designed for the **Base** blockchain (EVM-compatible).
- Wallet onboarding uses **thirdweb SDK v5** with **account abstraction** (Smart Accounts + sponsored gas) and supports both in-app wallets (email/passkey/social) and external wallets.

### Technology

- Next.js (App Router) + React + TypeScript
- Tailwind CSS
- thirdweb (ERC-1155 / ERC-20 integrations + Smart Accounts)
- hls.js (streaming playback)
- Vercel deployment

### How we build (quality + workflow)

- We keep changes small and reviewable, and always verify with audit/lint/build before shipping.
- We keep the UX stable across releases while maintaining compatibility with Node 24 + Yarn 4 for Vercel deployments.
- We treat this repo as an operational prototype: documented, repeatable, and ready to be extended for future campaigns and content libraries.

## 📜 Licensing & Usage

This project is protected under a [**Custom Limited License**](./LICENSE) [![License](https://img.shields.io/badge/license-Prof.NOTA%20Proprietary-orange.svg)](./LICENSE) by [Prof. NOTA & Prof. NOTA Inc.](https://nota.endhonesa.com/). See [PRICING.md](./PRICING.md) for usage tiers and [LICENSE](./LICENSE) for terms. Free usage is only allowed for cultural, and educational, for women- or child-focused projects approved by Prof. NOTA.

License available in multiple languages:

- 🏛️ [English (UK)](./licenses/LICENSE_en-GB.md)
- 🇮🇩 [Bahasa Indonesia](./licenses/LICENSE_ID.md)
- 🇺🇿 [Oʻzbekcha](./licenses/LICENSE_uz-Latn.md)
- 🇭🇰 [Cantonese – Hong Kong](./licenses/LICENSE_yue-Hant-HK.md)
- 🇲🇾 [Bahasa Malaysia](./licenses/LICENSE_ms-MY.md)
- 🇦🇪 [العربية – الإمارات](./licenses/LICENSE_ar-AE.md)

📩 Want to collaborate, deploy under your own brand, or inquire about licensing and permissions?  
Reach out to us at: [nota@endhonesa.com](mailto:nota@endhonesa.com)

---

## 📖 Manifestos

If you already have obtained the license, please read and understand the manifesto from [Prof. NOTA & Prof. NOTA Inc.](https://nota.endhonesa.com/) before starting to use it. Each deployment must respect the ideological foundation of Prof. NOTA Inc.

Manifestos are available in:

- 🏛️ [English (UK)](./manifestos/manifesto_en-GB.md)
- 🇮🇩 [Bahasa Indonesia](./manifestos/manifesto_id.md)
- 🇺🇿 [Oʻzbekcha](./manifestos/manifesto_uz-Latn.md)
- 🇭🇰 [Cantonese – Hong Kong](./manifestos/manifesto_yue-Hant-HK.md)
- 🇲🇾 [Bahasa Malaysia](./manifestos/manifesto_ms-MY.md)
- 🇦🇪 [العربية – الإمارات](./manifestos/manifesto_ar-AE.md)

---

## 🛠️ Getting Started

### 📦 Install dependencies

```bash
yarn install
```

### 🔍 Check outdated dependencies

```bash
yarn up -i
```

### ⬆️ Upgrade dependencies interactively

```bash
yarn up -R
```

### 🧹 Cleaning and re-install dependencies

```bash
rm -rf node_modules .yarn/install-state.gz && yarn install
```

### ▶️ Run development server

```bash
yarn dev
```

### 🧪 Lint and check all the code quality

```bash
yarn lint
```

### 🏗️ Build for production

```bash
yarn build
```

### 🔍 Preview the production

```bash
yarn start
```

---

## Evergreen Notes

- `@types/node` is pinned to **24.x** to match the Node 24 runtime (Vercel).
- Yarn is **4.x**; use `yarn outdated` for update review and `yarn npm audit --severity moderate` for security checks.
- Live parity check (memora.endhonesa.com): **All green** — no critical console errors, UX unchanged.

## 📦 Resources

- [Prof. NOTA Inc.](https://nota.endhonesa.com/)
- [Prof. NOTA Console](https://prompt.endhonesa.com/)
- [Prof. NOTA Tutor](https://baca.endhonesa.com/)
- [Prof. NOTA Artefacts](https://docs.endhonesa.com/)

---

## 🤝 Contributing

Your contribution is not only welcome — it's part of the protocol.

If you believe in the mission of PABRIKROTI and want to help improve it, follow these simple steps:

1. Fork this repository
2. Create a new branch (`feature/your-feature-name`)
3. Commit your changes mindfully
4. Open a pull request to the `preview` branch

Before submitting your PR, make sure to run:

```bash
yarn lint
```

To keep our code clean and consistent.

If you have questions, feel free to open an issue or reach out via the Prof. NOTA community Discord.

> ✊ You’re not just contributing code — you’re shaping how the people eat, learn, and resist.
>
> — Prof. NOTA

---

### 🫂 Join Prof. NOTA Discord

For feedback, questions, or cultural-technical collaboration, join Prof. NOTA discord at [https://discord.gg/5KrsT6MbFm](https://discord.gg/5KrsT6MbFm).

---

---

## Maintenance by Prof. NOTA Evergreen Standard

This repo is intended to stay evergreen while remaining production-safe.

### Current Baseline (Jan 2026)

- Runtime: Node **24.x** (Vercel-compatible; see `.nvmrc` and `package.json#engines`)
- Package manager: Yarn **4.12.0** (lockfile: `yarn.lock`)
- Types: `@types/node` **24.10.7** (pinned to match Node 24; 25.x intentionally deferred)
- Key packages: Next.js **16.1.4**, React **19.2.3**, thirdweb **5.118.0**, framer-motion **12.29.0**, hls.js **1.6.15**
- Deploy target: **Vercel auto-deploy from `main`**

### Monthly Evergreen Cycle (safe)

- `yarn install`
- `yarn up -R "*"`
- `yarn npm audit --severity moderate`
- `yarn lint`
- `yarn build`

### Quarterly Evergreen Cycle (major review)

- Review majors one at a time (framework/tooling), with a dedicated PR.
- If `@types/node` gets bumped, repin to **24.10.7**, then re-run audit/lint/build.
