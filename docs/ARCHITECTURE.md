# Architecture

## High-Level System Architecture

NexoLocal is a SaaS platform organized around a web application layer, a backend service layer, a relational data layer, and external integrations required for identity, communication, payments, and tax-oriented workflows.

## Core Layers

### Frontend

The frontend provides the public product experience as well as authenticated workspaces for operators, administrators, and company teams.

### Backend

The backend coordinates authentication, business rules, company operations, billing-related logic, permissions, and product workflows.

### Database

The data layer stores business, operational, subscription, support, and compliance-related information required by the platform.

### Service Integrations

NexoLocal connects with external providers for:

- email delivery
- OAuth-based authentication
- payments
- tax-oriented integrations

The public product direction also reflects continued investment in financial workflow expansion and resilience for tax-related operations.

## Product Architecture Principles

- Multi-company SaaS model
- Role-based access control
- Separation between public, private, platform, and company workflows
- Modular business domains for commercial and operational processes
- Support for subscription-driven company onboarding

## Public Documentation Scope

This public documentation intentionally stays at a high level. Internal route design, private service orchestration, data contracts, and implementation-specific operational details are not included here.
