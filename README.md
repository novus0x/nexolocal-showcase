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
- **Finance:** income and expense tracking, summaries, grouped entries, and export flows.
- **Cash management:** cash opening, closing, session tracking, and cash export flows.
- **Supplier management:** supplier creation, listing, reading, and updates.
- **Fiscal documents:** tax profile setup, fiscal series configuration, tax document records, and public document verification via `/check-ticket`.
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
- Company-side daily operations across products, suppliers, sales, finance, cash, settings, and tax configuration.
- Public verification of issued document information through a dedicated lookup flow.
- Support and invitation workflows for growing teams and multi-user company environments.

## Architecture

NexoLocal follows a two-application architecture:

- **Backend API:** a FastAPI application responsible for authentication, business rules, billing, company operations, tax-oriented workflows, and integrations.
- **Frontend:** an Express server-side rendered application that serves public pages, authentication flows, dashboards, and company/platform workspaces using Nunjucks views.
- **Database:** a relational model managed through SQLAlchemy, covering identity, access control, companies, billing, operations, support, tax data, and audit records.
- **Services layer:** dedicated internal services for email delivery, payment processing, and tax engine integration.
- **Modular components:** the system is organized into domain-specific route groups such as auth, platform, company, and general flows, which keeps responsibilities separated by business area.

## Tech Stack

### Frontend

- Node.js
- Express 5
- Nunjucks
- Tailwind CSS
- Vanilla JavaScript

### Backend

- Python 3.12
- FastAPI
- SQLAlchemy
- JWT-based session validation
- `bcrypt`
- `httpx`
- `aiosmtplib`
- ReportLab
- Jinja2

### Database

- Relational database mapped with SQLAlchemy models

### Infrastructure

- Docker
- Docker Compose
- SMTP integration
- Google OAuth integration
- Flow payment integration
- Tax engine integration

## System Modules

### Sales

Handles sale creation, customer lookup, sales listing, reports, and internal sale document generation.

### Inventory

Manages products, product batches, imports, and product update flows for company operations.

### Finance

Provides finance summaries, chart data, income and expense registration, and export functionality.

### Suppliers

Supports supplier creation, listing, detail retrieval, and updates.

### Tax Engine

Supports tax profile configuration, fiscal series, tax-oriented workflows, and tax document records.

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
│   ├── API.md
│   ├── ARCHITECTURE.md
│   ├── PAGE_CAPABILITIES.md
│   ├── DATABASE.md
│   ├── CHANGELOG.md
│   ├── MODULES.md
│   ├── README.md
│   └── SUMMARY.md
└── README.md
```

## Documentation

Detailed technical documentation is available in [`/docs`](./docs), including:

- Architecture overview
- Public API scope note
- Public data-layer scope note
- Module breakdown
- Functional page capabilities
- Project summary
- Release changelog

This repository is intended to act as a public-facing project overview and documentation hub.

## Development Status

NexoLocal is in active development. The documented platform already covers product discovery, authentication, onboarding, billing, platform administration, company operations, support flows, public document lookup, and active service management, while continuing to evolve as the product matures.

## Disclaimer

This repository contains documentation and project overview only. The core source code of NexoLocal is proprietary and not publicly available.

## Author

Created and maintained by `novus0x`.

For inquiries related to the project, use GitHub: [@novus0x](https://github.com/novus0x)
