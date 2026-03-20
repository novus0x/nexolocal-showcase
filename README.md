# NexoLocal

![Status](https://img.shields.io/badge/status-active%20development-0f766e)
![Repository](https://img.shields.io/badge/repository-public%20docs%20only-1f2937)
![Architecture](https://img.shields.io/badge/architecture-SaaS%20platform-0ea5e9)

**Operating system for local businesses.**

NexoLocal is a SaaS platform built to help local businesses manage sales, inventory, finance, cash operations, subscriptions, and tax-oriented workflows from a single system.

**Live site:** [https://nexolocal.floua.app](https://nexolocal.floua.app)

## Overview

NexoLocal is designed for local business operators that need more than a basic POS or spreadsheet-based workflow. It centralizes commercial operations, internal control, billing, onboarding, and company management in one platform.

The system addresses a common operational gap in small and growing businesses: disconnected tools for sales, stock, finance, customer follow-up, and fiscal compliance. NexoLocal brings these workflows together through a multi-company SaaS model with role-based access, platform administration, company workspaces, billing flows, and public tax document lookup.

## Key Features

- **Sales:** sale creation, customer lookup, reporting, and internal sale document generation.
- **Inventory:** product catalog, batch management, imports, and product updates.
- **Finance:** transaction tracking, finance containers, summaries, grouped entries, recurring operations, and export flows.
- **Cash management:** cash opening, closing, session tracking, and cash export flows.
- **Supplier management:** supplier creation, listing, reading, and updates.
- **Fiscal documents:** tax profile setup, fiscal series configuration, tax document records, public document verification via `/check-ticket`, and more resilient tax emission workflows.
- **Role-based permissions:** platform roles, permission catalog, company-scoped access, and guarded modules.
- **Multi-company architecture:** plan-based onboarding, company creation, subscriptions, billing history, and support for multiple companies per user.
- **Authentication and account lifecycle:** email/password authentication, Google OAuth, email verification, password recovery, and user password updates.
- **Post-sale service tracking:** active service lifecycle, validation/consumption flows, and customer linking.

## Platform Capabilities

At the business level, NexoLocal can support the full journey from product discovery to operational execution:

- Public product discovery with plan visibility and onboarding entry points.
- Account creation, login, email verification, and password recovery.
- Subscription management with first-company trial logic and paid flows for additional companies.
- Platform-side administration for users, roles, plans, companies, analytics, and staff support.
- Company-side daily operations across products, suppliers, sales, finance containers, recurring finance workflows, cash, settings, and tax configuration.
- Public verification of issued document information through a dedicated lookup flow.
- Support and invitation workflows for growing teams and multi-user company environments.

## Architecture

NexoLocal follows a two-application architecture:

- **Backend API:** a FastAPI application responsible for authentication, business rules, billing, company operations, tax-oriented workflows, and integrations.
- **Frontend:** a server-rendered web application that serves public pages, authentication flows, dashboards, and company/platform workspaces.
- **Database:** a relational model managed through SQLAlchemy, covering identity, access control, companies, billing, operations, support, tax data, and audit records.
- **Services layer:** dedicated internal services for email delivery, payment processing, and tax engine integration.
- **Modular components:** the system is organized into domain-specific route groups such as auth, platform, company, and general flows, which keeps responsibilities separated by business area.

## Tech Stack

### Frontend

- Node.js
- Express-based SSR architecture
- Server-rendered templating
- Modern web UI layer
- Vanilla JavaScript

### Backend

- Python 3.14
- FastAPI
- SQLAlchemy
- Token-based authentication
- Service-oriented backend architecture

### Database

- Relational database architecture

### Infrastructure

- Docker
- Docker Compose
- Email integration
- OAuth integration
- Payment integration
- Tax-oriented integration

## System Modules

### Sales

Handles sale creation, customer lookup, sales listing, reports, and internal sale document generation.

### Inventory

Manages products, product batches, imports, and product update flows for company operations.

### Finance

Provides finance summaries, chart data, income and expense registration, and export functionality.

Also supports broader finance workflows such as transaction management, finance containers, recurring financial operations, and richer finance views.

### Suppliers

Supports supplier creation, listing, detail retrieval, and updates.

### Tax Engine

Supports tax profile configuration, fiscal series, tax-oriented workflows, tax document records, and improved tax emission reliability.

### Authentication

Includes registration, login, logout, email verification, password recovery, Google OAuth, and session handling.

### Companies

Supports company onboarding, plan assignment, billing lifecycle, invitations, and company-scoped operations.

### Cash

Tracks cash sessions, opening and closing flows, and cash movement exports.

### Active Services

Tracks services sold after checkout, including activation, usage validation, expiration, and customer association.

### Platform Administration

Provides central management for users, roles, plans, companies, analytics, and support tickets.

## Project Structure

This public repository is documentation-first. The production source code is private, but the documented system is organized around the following structure:

```text
.
├── docs/
│   ├── ARCHITECTURE.md
│   ├── CHANGELOG.md
│   ├── MODULES.md
│   ├── PAGE_CAPABILITIES.md
│   ├── README.md
│   └── SUMMARY.md
└── README.md
```

## Documentation

Detailed technical documentation is available in [`/docs`](./docs), including:

- Architecture overview
- Module breakdown
- Functional page capabilities
- Project summary
- Release changelog: [`docs/CHANGELOG.md`](./docs/CHANGELOG.md)

This repository is intended to act as a public-facing project overview and documentation hub.

The published changelog represents the version history that has already been reviewed and approved for public disclosure. Additional internal versions or unreleased iterations may exist and may not yet be listed in this repository.

## Development Status

NexoLocal is in active development. The documented platform already covers product discovery, authentication, onboarding, billing, platform administration, company operations, support flows, public document lookup, and active service management, while continuing to evolve as the product matures.

Based on the public changelog, the latest documented additions include expanded finance workflows, finance containers, recurring finance improvements, stability-focused refinements, permission-related UI adjustments, and improved tax emission reliability.

## Disclaimer

This repository contains documentation and project overview only. The core source code of NexoLocal is proprietary and not publicly available.

## Author

Created and maintained by `novus0x`.

For inquiries related to the project, use GitHub: [@novus0x](https://github.com/novus0x)
