![Reflexx — A loyalty platform across web, mobile and API.](assets/banner.svg)

[Français](docs/CASE_STUDY.fr.md) · [Philippe Le Goff](https://github.com/PhilLeGoff) · [Portfolio](https://www.webbyphil.net/)

# Reflexx

A cross-platform loyalty product connecting merchant management interfaces, mobile customer journeys and a shared API. This case study focuses on the engineering of account access, loyalty transactions and delivery.

**Angular · Flutter · TypeScript · Node.js · Express · Prisma · PostgreSQL**

![Real Reflexx interface; see the screenshot context below](assets/interface.png)

*Screenshot context: real product marketing interface captured locally; inset dashboard figures are illustrative marketing content, not customer usage. The image does not establish live backend or production usage.*

## What it does

- Merchant programs, point balances, rewards and QR workflows.
- Web and mobile account journeys with role-based access.
- Transaction-safe point operations and an auditable loyalty history.
- Coordinated application delivery with database migrations and deployment workflows.

## Architecture

```mermaid
flowchart LR
  Web[Angular merchant web app] --> API[TypeScript Express API]
  Mobile[Flutter mobile app] --> API
  API --> Prisma[Prisma]
  Prisma --> DB[PostgreSQL]
  CI[GitHub Actions] --> API
  CI --> Web
```

## My contribution

I co-build Reflexx with two other engineers within a four-person venture, and coordinate the engineering team and technical roadmap. My work spans web/mobile journeys and API integration, including account access and loyalty workflows. The product is collaborative; this case study does not imply sole ownership of its code.

## Running and inspecting the project

No application source or hosted demo is distributed in this repository. The private development environment contains separate Angular, Flutter and Node.js applications backed by PostgreSQL. The screenshot shows the real public-facing product interface; it makes no claim about customer usage.

## Current state and limitations

Production infrastructure is deployed, while product areas remain at beta/pilot maturity. There are currently no customers or active users. This repository publishes the case study only; application source and operational configuration remain private.

## Credits

Reflexx is built by three engineers within a four-person venture. This documentation describes Philippe’s contribution and retains the collaborative product context.
