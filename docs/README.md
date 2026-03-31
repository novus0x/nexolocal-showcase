# NexoLocal

## Project Overview
NexoLocal is a production SaaS application for business operations, company onboarding, billing, sales, cash control, support, tax-oriented workflows, and active service tracking.

The current implementation covers public discovery, account creation, email verification, plan selection, company onboarding, platform administration, company management, supplier maintenance, public document lookup, and post-sale active service management.

The public product scope also includes a dedicated mobile application experience supported by a mobile-oriented integration layer.

## Main Features
- Email/password authentication and Google OAuth
- Account verification and password recovery
- Public landing page with plan discovery
- Private user area with dashboard, billing, invitations, and support
- Platform administration for users, roles, plans, companies, analytics, and support
- Company area for sales, sales analytics, inventory, services, suppliers, finance, finance containers, recurring finance workflows, cash, settings, and active services
- Tax-oriented setup for formal companies
- Subscription and onboarding flows for business workspaces
- Public document lookup
- Export-oriented cash and finance workflows
- Sales analytics and insight dashboards
- Recurring finance operations
- Finance containers and fund-level organization
- Independent product and service workflows
- Team management, invitations, and role-based collaboration
- Plan feature system
- CSV exports for products and services
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

### Database
- Relational database architecture

### Services and Integrations
- Email integration
- OAuth integration
- Tax-oriented integration
- Payment integration

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

The latest public changelog entries reflect continued expansion of the finance area, continued UI refinement, improved tax emission reliability, the separation of product and service workflows, sales analytics, team-oriented workspace features such as roles, invitations, plan features, and CSV exports, plus the introduction of a dedicated mobile app and integration layer.
