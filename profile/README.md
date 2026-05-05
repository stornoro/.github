<div align="center">

<img src="https://storno.ro/images/logo-light.png#gh-dark-mode-only" alt="Storno.ro" height="64" />
<img src="https://storno.ro/images/logo-dark.png#gh-light-mode-only" alt="Storno.ro" height="64" />

# Storno.ro

**Open-source invoicing platform for Romanian businesses.**
e-Factura ANAF · multi-company · POS · mobile · API · MCP for AI assistants.

[Website](https://storno.ro) ·
[App](https://app.storno.ro) ·
[Docs](https://docs.storno.ro) ·
[Self-hosting](https://get.storno.ro) ·
[Status](https://status.storno.ro) ·
[MCP](https://mcp.storno.ro)

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-2563eb?style=flat-square)](https://github.com/stornoro/storno/blob/main/LICENSE)
[![Self-hostable](https://img.shields.io/badge/self--hostable-yes-10b981?style=flat-square)](https://get.storno.ro)
[![ANAF e-Factura](https://img.shields.io/badge/ANAF%20e--Factura-integrated-2563eb?style=flat-square)](https://docs.storno.ro/concepts/einvoice-integration)
[![Made in Romania](https://img.shields.io/badge/made%20in-%F0%9F%87%B7%F0%9F%87%B4-EE6E1F?style=flat-square)](https://storno.ro)

</div>

---

## What is Storno.ro

A complete invoicing platform built for the Romanian fiscal stack — e-Factura, ANAF SPV, conformity with **OUG 130/2021**. Same codebase, two ways to use it:

- **[storno.ro](https://storno.ro)** — fully managed cloud, 14 days free, no card.
- **[get.storno.ro](https://get.storno.ro)** — self-host on your own server with one Docker command. Same features as cloud, your data never leaves your infrastructure.

```bash
curl -fsSL https://get.storno.ro | bash
```

## Repositories

|   | Repo | What it does |
|---|---|---|
| 📦 | **[storno](https://github.com/stornoro/storno)** | Core monorepo — Symfony 7 backend + Nuxt 4 frontend |
| 📚 | **[docs](https://github.com/stornoro/docs)** | Documentation site — self-hosting guides, API reference |
| 🤖 | **[storno-cli](https://github.com/stornoro/storno-cli)** | CLI + MCP server (228 tools) — drive Storno from Claude / Cursor / Windsurf |
| 💳 | **[stripe-app](https://github.com/stornoro/stripe-app)** | Stripe Marketplace app — auto e-Factura from Stripe payments |
| 📊 | **[status](https://github.com/stornoro/status)** | Real-time uptime monitoring & public status page |

### E-commerce & framework integrations

|   | Repo | Platform |
|---|---|---|
| 🛒 | **[woocommerce-storno-invoicing](https://github.com/stornoro/woocommerce-storno-invoicing)** | WooCommerce |
| 🛒 | **[prestashop-storno-invoicing](https://github.com/stornoro/prestashop-storno-invoicing)** | PrestaShop |
| 🛒 | **[shopify-storno-invoicing](https://github.com/stornoro/shopify-storno-invoicing)** | Shopify |
| 🛒 | **[magento-storno-invoicing](https://github.com/stornoro/magento-storno-invoicing)** | Magento 2 |
| 🛒 | **[opencart-storno-invoicing](https://github.com/stornoro/opencart-storno-invoicing)** | OpenCart |
| 🛒 | **[cscart-storno-invoicing](https://github.com/stornoro/cscart-storno-invoicing)** | CS-Cart 4.15+ |
| 🐘 | **[laravel-storno](https://github.com/stornoro/laravel-storno)** | Laravel package |

## Features

- **e-Factura ANAF** — automatic SPV submission and retrieval, token auto-refresh, status sync to dashboard
- **Multi-company native** — manage unlimited companies under one account, isolated data per CIF
- **POS module** — sell on mobile with barcode scanner, mixed payments (cash + card), refunds, SGR deposit returns, full offline support
- **Recurring invoices** — set frequency, recipients, payment links once
- **Stripe payments** — invoice link in every email, auto-reconcile when paid
- **REST API + MCP** — 228 tools exposed via Model Context Protocol for AI assistants
- **Mobile native** — iOS + Android, biometric auth, push notifications, real-time sync
- **Open source** — self-host on your own infrastructure, datele rămân la tine

## AI integrations

Storno.ro exposes its full API as MCP tools for AI assistants. Add it once and your AI can manage invoices in plain language.

```
https://mcp.storno.ro/mcp
```

Works with **Claude Desktop**, **Claude Code**, **Cursor**, **Windsurf**, **Zed**, and any other MCP-compatible client. Install instructions: [mcp.storno.ro](https://mcp.storno.ro).

## Tech stack

[![Symfony](https://img.shields.io/badge/Symfony-7-000000?style=flat-square&logo=symfony)](https://symfony.com)
[![Nuxt](https://img.shields.io/badge/Nuxt-4-00DC82?style=flat-square&logo=nuxt.js)](https://nuxt.com)
[![Vue](https://img.shields.io/badge/Vue-3-4FC08D?style=flat-square&logo=vue.js)](https://vuejs.org)
[![React Native](https://img.shields.io/badge/React%20Native-Mobile-61DAFB?style=flat-square&logo=react)](https://reactnative.dev)
[![PHP](https://img.shields.io/badge/PHP-8.4-777BB4?style=flat-square&logo=php)](https://php.net)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript)](https://typescriptlang.org)
[![MariaDB](https://img.shields.io/badge/MariaDB-blue?style=flat-square&logo=mariadb)](https://mariadb.org)
[![Docker](https://img.shields.io/badge/Docker-ready-2496ED?style=flat-square&logo=docker)](https://docker.com)

## Licensing

- **Community Edition** (self-host) — AGPL-3.0, free forever, full feature set
- **Cloud / Commercial / OEM** — paid tiers from 19 RON/month, [pricing](https://storno.ro/pricing)

Repository licenses are listed in each project's `LICENSE` file.

## Contributing

We welcome PRs across the ecosystem — backend bug fixes, integrations for new e-commerce platforms, MCP tool additions, translations.

- Read the [contributing guide](https://docs.storno.ro/contributing-guide) before opening a PR
- Bugs and feature requests: [github.com/stornoro/storno/issues](https://github.com/stornoro/storno/issues)
- Security: please report responsibly via [security policy](https://github.com/stornoro/storno/security/policy)

## Connect

[storno.ro](https://storno.ro) · [contact@storno.ro](mailto:contact@storno.ro) · [Facebook](https://www.facebook.com/storno.ro)

<sub>© Storno.ro · Built in Romania for Romanian businesses</sub>
