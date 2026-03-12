# NexoLocal

## Project Overview
NexoLocal is a production SaaS application for business operations, company onboarding, billing, sales, cash control, support, tax-oriented workflows, and active service tracking.

The current implementation covers public discovery, account creation, email verification, plan selection, company onboarding, platform administration, company management, supplier maintenance, public document lookup, and post-sale active service management.

## Main Features
- Email/password authentication and Google OAuth
- Account verification and password recovery
- Public landing page with plan discovery
- Private user area with dashboard, billing, invitations, and support
- Platform administration for users, roles, plans, companies, analytics, and support
- Company area for sales, inventory, suppliers, finance, cash, settings, and active services
- Tax-oriented setup for formal companies
- Subscription and onboarding flows for business workspaces
- Public document lookup
- Export-oriented cash and finance workflows

## Tech Stack
### Backend
- Python 3.12
- FastAPI
- SQLAlchemy ORM
- JWT-based session validation
- `bcrypt`
- `httpx`
- `aiosmtplib`
- ReportLab
- Jinja2

### Frontend
- Node.js
- Express 5
- Nunjucks
- Tailwind CSS
- Vanilla browser JavaScript

### Database
- Relational schema mapped with SQLAlchemy models

### Services and Integrations
- SMTP email delivery
- Google OAuth
- Tax-oriented integration
- Flow payment integration

## Public Documentation Scope

This repository is public for product documentation and project overview purposes. It does not include the proprietary implementation, deployment instructions, private API contracts, or infrastructure secrets of the production system.

## Technology Overview

NexoLocal is documented as a modern web platform built with:

- Python and FastAPI on the backend
- Node.js, Express SSR, and Nunjucks on the frontend
- SQLAlchemy-managed relational persistence
- External integrations for email, OAuth, payments, and tax-oriented workflows

## Folder Structure Overview
- `docs/`: public project documentation

## Documentation Files
- `docs/ARCHITECTURE.md`
- `docs/DATABASE.md`
- `docs/MODULES.md`
- `docs/API.md`
- `docs/PAGE_CAPABILITIES.md`
- `docs/SUMMARY.md`
- `docs/CHANGELOG.md`

## Documentation Note
This documentation is intended as a public-facing overview of the product and its evolution. It describes the platform at a business and architecture level without exposing proprietary implementation details.
