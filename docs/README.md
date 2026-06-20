# NexoLocal

## Project Overview
NexoLocal is a production SaaS application for business operations, company onboarding, billing, sales, analytics, production, orders, customer management, finance and cash control, support, reporting, tax-oriented workflows, and active service tracking.

The current implementation covers public discovery, account creation, email verification, plan selection, company onboarding, platform administration, company management, customer management, supplier maintenance, production and order workflows, public document lookup, support lifecycle handling, knowledge base publishing, reporting exports, post-sale active service management, and expanded treasury-oriented finance and cash workflows.

The public product scope also includes a dedicated mobile application experience supported by a mobile-oriented integration layer.

## Main Features
- Email/password authentication and Google OAuth
- Account verification and password recovery
- Public landing page with plan discovery
- Private user area with dashboard, billing, invitations, and support
- Platform administration for users, roles, plans, companies, analytics, changelog operations, and support
- Company area for customers, sales, business analytics, inventory, services, production, orders, suppliers, finance, finance containers, financial planning workflows, recurring finance workflows, cash, settings, knowledge base content, and active services
- Tax-oriented setup for formal companies
- Subscription and onboarding flows for business workspaces
- Public document lookup
- Export-oriented sales, cash, and finance workflows
- Unified PDF reporting for sales, finance, and cash reports
- Period-segmented finance PDF reports with grouped subtotals
- Customer records with history across sales and services
- Sales analytics and insight dashboards
- Executive analytics with predictions, risks, goals, business health scoring, and PDF exports
- Recurring finance operations
- Finance containers and fund-level organization
- Fund reset cycles for finance containers
- Budgets, obligations, financial calendar, projections, and finance categories
- Main cash and subcash session management
- Consolidated cash reporting and treasury-oriented business rules
- Independent product and service workflows
- Production recipes, work orders, costing, and inventory transformation workflows
- Orders and fulfillment workflows with sales and cash integration
- Team management, invitations, and role-based collaboration
- Plan feature system
- CSV exports for products and services
- CSV exports for customers
- Commission PDF exports with export permissions
- Support ticket lifecycle management
- Public knowledge base and support portal
- Changelog publishing, notifications, read tracking, and update history
- Mobile application experience
- Reusable frontend design system with tokens, themes, and utilities
- Full light mode support
- Async list infrastructure for pagination, filtering, partial HTML updates, and persistent URL state

## Tech Stack
### Backend
- Python 3.14
- FastAPI
- SQLAlchemy
- Token-based authentication
- Service-oriented backend architecture

### Frontend
- Node.js
- Express-based SSR architecture
- Server-rendered templating
- Modern web UI layer
- Vanilla JavaScript
- Reusable design system architecture
- HTML template-based report rendering

### Database
- Relational database architecture

### Services and Integrations
- Email integration
- OAuth integration
- Tax-oriented integration
- Payment integration
- WeasyPrint-based PDF reporting

## Public Documentation Scope

This repository is public for product documentation and project overview purposes. It does not include the proprietary implementation, deployment instructions, private API contracts, or infrastructure secrets of the production system.

## Technology Overview

NexoLocal is documented as a modern web platform built with:

- Python and FastAPI on the backend
- Node.js and a server-rendered frontend architecture
- Relational data persistence
- External integrations for email, OAuth, payments, and tax-oriented workflows

## Folder Structure Overview
- `docs/`: public project documentation

## Documentation Files
- `docs/ARCHITECTURE.md`
- `docs/MODULES.md`
- `docs/PAGE_CAPABILITIES.md`
- `docs/SUMMARY.md`
- `docs/CHANGELOG.md`

## Documentation Note
This documentation is intended as a public-facing overview of the product and its evolution. It describes the platform at a business and architecture level without exposing proprietary implementation details.

The latest public changelog entries reflect the introduction of executive analytics, production and recipe management, orders and fulfillment, financial planning workflows, supplier and finance UX refinements, a public knowledge base, and a changelog management system with notifications and read tracking.
