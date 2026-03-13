# Changelog

This file summarizes the documented release history of NexoLocal.

| version | name | description | lines |
| --- | --- | --- | ---: |
| 1.0.0 | Initial release | Initial project structure and core SaaS architecture | 15230 |
| 1.1.0 | Google auth and product logic improvements | Add Google OAuth authentication and improve product logic | 15714 |
| 1.2.0 | Email service and legal compliance | Introduce email service and legal compliance updates | 16214 |
| 1.2.1 | Remove Alembic | Migrate from Alembic to manual database schema management | 16118 |
| 1.3.0 | Account recovery and password reset | Implement account recovery and password reset flow | 17207 |
| 1.4.0 | Bulk sales and timezone support | Add bulk sales capability and server timezone handling | 17440 |
| 1.4.1 | Fix date inconsistencies | Fix issues related to date handling across the system | 17451 |
| 1.5.0 | Platform upgrades (roles and users) | Add platform administration for assigning and managing users and roles | 18267 |
| 1.5.1 | Platform user edit fix | Fix platform user editing and adjust UI behaviour | 18303 |
| 1.5.2 | General bug fixes and UI improvements | Improve stability and adjust various UI components | 18472 |
| 1.6.0 | Basic suppliers management | Introduce supplier records and basic supplier management | 19166 |
| 1.7.0 | Supplier-product integration and landing page | Link suppliers to products and add first landing page | 19789 |
| 1.8.0 | Ticket-based support system | Introduce internal ticket-based support system | 21907 |
| 1.8.1 | Email verification template | Add email verification template for user accounts | 22004 |
| 1.8.2 | i18n configuration completion | Complete internationalization configuration | 22378 |
| 1.9.0 | Billing foundation and tax engine structure | Introduce billing foundation and tax engine architecture | 23259 |
| 1.10.0 | Company fiscal profile support | Add company profile editing and fiscal data support | 23518 |
| 1.11.0 | Tax engine profile linking | Link tax engine profile with fiscal settings | 24151 |
| 1.11.1 | Audit model introduction | Introduce audit logging model for tracking actions | 24336 |
| 1.12.0 | Dynamic subscription plans | Implement dynamic subscription plans integrated with roles | 25387 |
| 1.13.0 | Billing trial system and dashboard | Introduce trial system billing flow and account verification | 26661 |
| 1.13.1 | UI fixes | Minor UI fixes and layout adjustments | 26654 |
| 1.13.2 | Fix tax_included and stock alerts | Resolve tax_included calculation and stock alert issues | 26639 |
| 1.13.3 | General bug fixes | Small stability fixes across the system | 26640 |
| 1.14.0 | Receipt issuance system | Add automatic receipt issuance and fix decimal precision | 27461 |
| 1.14.1 | Manual receipt issuance support | Enable manual receipt issuance alongside automatic mode | 27461 |
| 1.14.2 | Navigation and dashboard improvements | Improve navigation clarity and dashboard experience | 27543 |
| 1.14.3 | Finance UI improvements | Improve finance entry UI with income and expense toggle buttons | 27598 |
| 1.14.4 | Sidebar visual improvements | Improve sidebar spacing and icon alignment | 27650 |
| 1.14.5 | Dashboard company retrieval improvement | Improve dashboard with proper user company retrieval | 27718 |
| 1.14.6 | Display trial status | Show company trial status in plan settings | 27730 |
| 1.14.7 | Tax API production configuration | Add production environment configuration for tax API | 27967 |
| 1.14.8 | Company ID bug fix | Fix company ID handling bug | 27969 |
| 1.14.9 | Payment fee provider migration | Migrate payment fee service from MercadoPago to Flow | 27969 |
| 1.15.0 | Initial payment support | Introduce payment support through Flow integration | 28324 |
| 1.16.0 | Billing transaction history | Add billing transaction history view | 28453 |
| 1.17.0 | Ticket endpoint improvements | Enhance ticket endpoint behaviour and printing workflow | 28511 |
| 1.18.0 | Public ticket lookup and QR verification | Enable public verification of receipts using QR codes | 28746 |
| 1.19.0 | Fiscal numbering alignment | Align fiscal numbering with tax series configuration | 28775 |
| 1.19.1 | Centralized subscription validation | Centralize company subscription validation logic | 28891 |
| 1.20.0 | Subscription renewal support | Add support for subscription renewal flow | 29411 |
| 1.20.1 | Expired company handling | Improve handling of expired companies and billing redirection | 29469 |
| 1.20.2 | Product update flow | Add product update workflow in management interface | 29884 |
| 1.20.3 | Service duration restrictions | Enforce service duration validation and inventory restrictions | 29908 |
| 1.21.0 | Customer records and sales autocomplete | Introduce company customer records and sales autocomplete | 30281 |
| 1.22.0 | Active service lifecycle | Introduce lifecycle management for sold services | 31890 |
| 1.22.1 | UUID migration v4 to v7 | Migrate UUID generation from v4 to v7 | 31890 |
| 1.22.2 | Email verification hardening | Strengthen email verification and sanitize support HTML content | 32012 |
| 1.22.3 | Ticket access control improvements | Improve ticket access control and billing error handling | 32027 |
| 1.22.4 | Date handling fixes | Fix date parsing and handling issues | 32032 |
| 1.23.0 | Filtered CSV and PDF exports | Introduce CSV and PDF export with filtering support | 32780 |
| 1.23.1 | PDF export refinements | Refine PDF export layout and summary formatting | 32809 |
| 1.24.0 | Cash closing PDF export | Add exportable PDF report for cash closing sessions | 33150 |
| 1.24.1 | Cash report improvements | Improved cash closing report layout | 33199 |
| 1.25.0 | Permission-aware dashboard | Dashboard adapts to permissions | 33534 |
| 1.26.0 | Plan summary & landing | Plan summary field and landing redesign | 34079 |
| 1.26.1 | Auth UI improvements | Authentication UI improvements | 34123 |
| 1.27.0 | Suppliers improvements | Suppliers module improvements | 34762 |
| 1.27.1 | Suppliers backend | Backend additions for suppliers module | 34881 |
| 1.28.0 | Finance module improvements | Added full finance transactions workflow: movements page with pagination, read view, update flow, improved receipt handling and navigation | 36148 |
| 1.29.0 | Recurring finance system | Implemented recurring financial operations with full CRUD, improved UI, and a background worker that processes recurring entries every 30 minutes | 38589 |
