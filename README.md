# NexoLocal

![Status](https://img.shields.io/badge/status-active%20development-0f766e)
![Repository](https://img.shields.io/badge/repository-public%20docs%20only-1f2937)
![Architecture](https://img.shields.io/badge/architecture-SaaS%20platform-0ea5e9)

**Operating system for local businesses.**

NexoLocal is a SaaS platform built to help local businesses manage sales, customers, inventory, finance, treasury and cash operations, subscriptions, support, reporting, and tax-oriented workflows from a single system.

**Live site:** [https://nexolocal.floua.app](https://nexolocal.floua.app)

## Overview

NexoLocal is designed for local business operators that need more than a basic POS or spreadsheet-based workflow. It centralizes commercial operations, internal control, billing, onboarding, and company management in one platform.

The system addresses a common operational gap in small and growing businesses: disconnected tools for sales, customer follow-up, stock, finance, treasury control, support, reporting, and fiscal compliance. NexoLocal brings these workflows together through a multi-company SaaS model with role-based access, platform administration, company workspaces, billing flows, and public tax document lookup.

The platform now extends beyond the web experience with a dedicated mobile application layer, reinforcing NexoLocal as a multi-surface operating system for local businesses.

## Key Features

- **Sales:** sale creation, customer lookup, reporting, PDF report exports, and internal sale document generation.
- **Business analytics:** real-time sales insights, executive dashboards, predictions, goals, risks, business health scoring, and PDF exports.
- **Customer management:** customer listing, detail, updates, CSV export, and sales/service history.
- **Inventory:** product catalog, batch management, imports, and product updates.
- **Services:** independent service-oriented workflows alongside product operations.
- **Production operations:** recipes, work orders, costing, inventory transformations, and production supplies organization.
- **Orders and fulfillment:** order lifecycle workflows with sales, cash, and operational fulfillment integration.
- **Finance:** transaction tracking, finance containers, summaries, grouped entries, recurring operations, fund reset cycles, segmented reports, and unified PDF/CSV export flows.
- **Financial planning:** budgets, obligations, financial calendar, projections, categories, commissions, and referrals reporting.
- **Cash management:** main cash and subcash sessions, cash opening and closing, user-level session tracking, consolidated reporting, treasury-oriented rules, and unified PDF export flows.
- **Supplier management:** supplier creation, listing, reading, and updates.
- **Fiscal documents:** tax profile setup, fiscal series configuration, tax document records, public document verification via `/check-ticket`, and more resilient tax emission workflows.
- **Role-based permissions:** platform roles, permission catalog, company-scoped access, and guarded modules.
- **Team management:** company roles, invitations, and team-oriented workspace collaboration.
- **Knowledge base:** internal content management plus a public support and documentation portal.
- **Product updates center:** changelog publishing, notifications, read tracking, and release history visibility.
- **Multi-company architecture:** plan-based onboarding, company creation, subscriptions, billing history, and support for multiple companies per user.
- **Plan feature system:** plan-driven feature organization for company capabilities.
- **Authentication and account lifecycle:** email/password authentication, Google OAuth, email verification, password recovery, and user password updates.
- **CSV exports:** export support for product and service datasets.
- **Post-sale service tracking:** active service lifecycle, validation/consumption flows, service activation integration, and customer linking.
- **Support lifecycle:** ticket states, closing, reopening, and platform support follow-up.
- **Mobile app experience:** dedicated mobile workflows backed by a mobile-focused integration layer.
- **Frontend design system:** reusable tokens, themes, and utilities for consistent interface architecture.
- **Light mode support:** full light-theme coverage across the platform experience.
- **Async list infrastructure:** reusable pagination, filtering, partial HTML updates, and persistent URL state handling through `NexoAsyncList`.

## Platform Capabilities

At the business level, NexoLocal can support the full journey from product discovery to operational execution:

- Public product discovery with plan visibility and onboarding entry points.
- Account creation, login, email verification, and password recovery.
- Subscription management with first-company trial logic and paid flows for additional companies.
- Platform-side administration for users, roles, plans, companies, analytics, and staff support.
- Company-side daily operations across customers, products, services, suppliers, sales, analytics, production, orders, finance containers, financial planning workflows, recurring finance workflows, fund reset cycles, cash, knowledge base content, settings, and tax configuration.
- Team collaboration through roles, invitations, and plan-aware workspace capabilities.
- Mobile access through a dedicated application experience with module coverage aligned to business operations.
- Public verification of issued document information through a dedicated lookup flow.
- Support lifecycle and invitation workflows for growing teams and multi-user company environments.
- Async list-driven module views with filtering, pagination, and partial updates.
- Light mode support, compact-sidebar behavior that preserves user navigation state, and a branded public ticket verification experience.

## Architecture

NexoLocal follows a multi-surface SaaS architecture:

- **Backend API:** a FastAPI application responsible for authentication, business rules, billing, company operations, tax-oriented workflows, and integrations.
- **Web frontend:** a server-rendered web application that serves public pages, authentication flows, dashboards, and company/platform workspaces with a reusable design system and async UI patterns.
- **Mobile app layer:** a dedicated mobile experience backed by a mobile-oriented API/BFF integration layer.
- **Database:** a relational model managed through SQLAlchemy, covering identity, access control, companies, billing, operations, support, tax data, and audit records.
- **Services layer:** dedicated internal services for email delivery, payment processing, tax engine integration, treasury-oriented finance coordination, and HTML-to-PDF reporting.
- **Modular components:** the system is organized into domain-specific route groups such as auth, platform, company, and general flows, which keeps responsibilities separated by business area.

## Tech Stack

### Frontend

- Node.js
- Express-based SSR architecture
- Server-rendered templating
- Modern web UI layer
- Vanilla JavaScript
- Mobile application layer
- Reusable design system architecture
- HTML template-based report rendering

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
- WeasyPrint-based PDF reporting

## System Modules

### Sales

Handles sale creation, customer lookup, sales listing, reports, PDF exports, and internal sale document generation.

Also supports analytics-oriented dashboards with executive insights, business health scoring, predictions, goals, risks, and PDF exports.

### Inventory

Manages products, product batches, imports, and product update flows for company operations.

### Customers

Manages customer records, detail views, updates, CSV exports, and historical visibility across sales and services.

### Services

Supports service-specific workflows separated from product operations, allowing the platform to handle each business flow more clearly.

### Finance

Provides finance summaries, chart data, income and expense registration, and export functionality.

Also supports broader finance workflows such as transaction management, finance containers, recurring financial operations, richer finance views, fund reset cycles, segmented PDF reporting, and grouped subtotals by cycle period.

This scope now also includes budgeting, obligations, projections, calendar-based planning, finance categories, commission exports, and refined permissions around financial reporting.

### Production

Supports recipes, work orders, costing visibility, production supplies organization, and inventory transformation workflows.

### Orders

Supports operational order management, fulfillment flows, realtime search, and integration with sales and cash processes.

### Suppliers

Supports supplier creation, listing, detail retrieval, and updates.

This area also includes a refreshed interface aligned with the platform design system.

### Tax Engine

Supports tax profile configuration, fiscal series, tax-oriented workflows, tax document records, and improved tax emission reliability.

### Authentication

Includes registration, login, logout, email verification, password recovery, Google OAuth, and session handling.

### Companies

Supports company onboarding, plan assignment, billing lifecycle, invitations, team management, and company-scoped operations.

This scope also extends to mobile-oriented access patterns for supported business modules.

### Cash

Tracks main cash and subcash sessions, opening and closing flows, user-level cash control, consolidated reporting, treasury-oriented rules, and cash movement exports through the unified PDF reporting system.

### Active Services

Tracks services sold after checkout, including activation, usage validation, expiration, and customer association.

### Platform Administration

Provides central management for users, roles, plans, plan features, companies, analytics, and support tickets with state-based support lifecycle handling.

It also includes a platform dashboard and dynamic plan-highlighting support for commercial visibility.

### Knowledge Base

Provides category and article management, public documentation publishing, and sanitized content rendering for support-oriented self-service.

### Updates Center

Provides changelog publishing, scheduled release visibility, notification delivery, read tracking, and update history browsing.

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

Based on the public changelog, the latest documented additions include executive analytics with PDF exports, production and recipe workflows, order fulfillment, financial planning tools, supplier and finance UX refinements, a public knowledge base, and a changelog management system with notifications and read tracking.

## Disclaimer

This repository contains documentation and project overview only. The core source code of NexoLocal is proprietary and not publicly available.

## Author

Created and maintained by `novus0x`.

For inquiries related to the project, use GitHub: [@novus0x](https://github.com/novus0x)
