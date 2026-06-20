# Architecture

## High-Level System Architecture

NexoLocal is a SaaS platform organized around a web application layer, a mobile application layer, a backend service layer, a relational data layer, a reporting layer, and external integrations required for identity, communication, payments, and tax-oriented workflows.

## Core Layers

### Frontend

The frontend provides the public product experience as well as authenticated workspaces for operators, administrators, and company teams.

It also presents report configuration and export flows for sales, finance, and cash operations.

The frontend direction now includes a reusable design system architecture with tokens, themes, and utilities, full light mode support, async list infrastructure for filtering and pagination, compact-sidebar behavior that preserves user navigation state, and branded public experiences for document verification, support content, and product updates.

### Mobile App

The mobile layer extends the platform to dedicated app-based workflows for supported business modules.

### Backend

The backend coordinates authentication, business rules, company operations, billing-related logic, permissions, customer workflows, support lifecycle handling, production and order workflows, analytics, and product workflows.

It also supports a mobile-oriented integration layer for app experiences.

The service layer also coordinates treasury-oriented finance and cash rules, including fund reset cycles, budgeting and projection workflows, main cash and subcash handling, and reporting-ready operational aggregation.

### Database

The data layer stores customer, business, operational, subscription, support, documentation, update-history, reporting, and compliance-related information required by the platform.

### Reporting

The reporting layer uses HTML templates and WeasyPrint to generate unified PDF reports across sales, finance, and cash workflows.

It also supports period-based segmentation for finance reports, grouped subtotals by cycle period, opener visibility in cash exports, and refined pagination and layout behavior for generated PDFs.

### Service Integrations

NexoLocal connects with external providers for:

- email delivery
- OAuth-based authentication
- payments
- tax-oriented integrations

The public product direction also reflects continued investment in executive analytics, production and fulfillment workflows, treasury expansion, documentation self-service, product-update visibility, segmented reporting, reusable frontend infrastructure, async interaction patterns, and resilience for tax-related operations.

## Product Architecture Principles

- Multi-company SaaS model
- Role-based access control
- Separation between public, private, platform, and company workflows
- Modular business domains for commercial and operational processes
- Support for subscription-driven company onboarding
- Unified report generation across business modules
- Reusable interface primitives and theme-driven UI consistency
- Async-first list and filtering patterns for operational modules

## Public Documentation Scope

This public documentation intentionally stays at a high level. Internal route design, private service orchestration, data contracts, and implementation-specific operational details are not included here.
