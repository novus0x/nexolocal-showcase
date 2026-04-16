# NexoLocal

## Project Overview
NexoLocal is a production SaaS application for business operations, company onboarding, billing, sales, customer management, cash control, support, reporting, tax-oriented workflows, and active service tracking.

The current implementation covers public discovery, account creation, email verification, plan selection, company onboarding, platform administration, company management, customer management, supplier maintenance, public document lookup, support lifecycle handling, reporting exports, and post-sale active service management.

The public product scope also includes a dedicated mobile application experience supported by a mobile-oriented integration layer.

## Main Features
- Email/password authentication and Google OAuth
- Account verification and password recovery
- Public landing page with plan discovery
- Private user area with dashboard, billing, invitations, and support
- Platform administration for users, roles, plans, companies, analytics, and support
- Company area for customers, sales, sales analytics, inventory, services, suppliers, finance, finance containers, recurring finance workflows, cash, settings, and active services
- Tax-oriented setup for formal companies
- Subscription and onboarding flows for business workspaces
- Public document lookup
- Export-oriented sales, cash, and finance workflows
- Unified PDF reporting for sales, finance, and cash reports
- Customer records with history across sales and services
- Sales analytics and insight dashboards
- Recurring finance operations
- Finance containers and fund-level organization
- Independent product and service workflows
- Team management, invitations, and role-based collaboration
- Plan feature system
- CSV exports for products and services
- CSV exports for customers
- Support ticket lifecycle management
- Mobile application experience

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

The latest public changelog entries reflect the introduction of the mobile app and API layer, a complete customer management module, support ticket lifecycle improvements, sales PDF export, and the migration of sales, finance, and cash reports into a unified WeasyPrint-based PDF reporting system.
