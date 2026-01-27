# Nuvei Developer Documentation Structure

## Overview

This Mintlify documentation site provides comprehensive coverage of Nuvei's REST API 2.0 integration with clear entry points for legacy products.

## Directory Structure

```
rest-2-poc/
├── mint.json                    # Mintlify configuration
├── portal/                      # Cross-product portal pages
│   └── choose-integration.mdx   # Integration method comparison
├── rest-2/                      # REST API 2.0 documentation
│   ├── introduction.mdx         # REST 2.0 landing page
│   ├── whats-new.mdx
│   ├── quickstart.mdx
│   ├── authentication.mdx
│   ├── testing.mdx
│   ├── error-codes.mdx
│   ├── changelog.mdx
│   ├── concepts/                # Core concepts
│   │   ├── restful-structure.mdx
│   │   ├── environments.mdx
│   │   ├── record-ids.mdx
│   │   └── transaction-types.mdx
│   └── guides/                  # Payment method guides
│       ├── overview.mdx
│       ├── cards/               # Card payments
│       │   ├── non-3ds.mdx
│       │   ├── 3ds-flow.mdx
│       │   └── tokenization.mdx
│       ├── wallets/             # Digital wallets
│       │   ├── apple-pay.mdx
│       │   └── google-pay.mdx
│       ├── bank/                # Bank transfers
│       │   └── ach.mdx
│       ├── operations/          # Payment operations
│       │   ├── refunds.mdx
│       │   ├── voids.mdx
│       │   └── settlements.mdx
│       └── webhooks/            # Webhook integration
│           ├── overview.mdx
│           └── handling.mdx
├── api-reference/               # API endpoint reference
│   ├── overview.mdx
│   ├── payments/                # Payment endpoints
│   │   ├── create-payment.mdx
│   │   ├── fingerprint.mdx
│   │   ├── challenge.mdx
│   │   ├── refund.mdx
│   │   ├── void.mdx
│   │   └── settle.mdx
│   └── accounts/                # Account endpoints
│       └── get-payment-tokens.mdx
└── legacy/                      # Legacy product entry points
    ├── rest-1.mdx               # REST 1.0 overview + link-out
    ├── web-sdk.mdx              # Web SDK overview + link-out
    └── simply-connect.mdx       # Simply Connect overview + link-out
```

## Navigation Structure

### Tabs
1. **REST API 2.0** - Primary integration method (rest-2/)
2. **API Reference** - Endpoint documentation (api-reference/)
3. **Legacy Docs** - Legacy product entry points (legacy/)

### Groups
- **Home**: Integration method comparison
- **Getting Started**: Introduction, quickstart, authentication
- **Core Concepts**: RESTful structure, environments, record IDs, transaction types
- **Payment Methods**: Cards, wallets, bank transfers
- **Operations**: Refunds, voids, settlements
- **Webhooks**: Overview and handling
- **Resources**: Testing, error codes, changelog
- **API Reference**: Overview
- **Payments**: Payment endpoints
- **Accounts**: Account endpoints
- **Legacy Documentation**: REST 1.0, Web SDK, Simply Connect

## File Count

- **Total MDX files**: 36
  - rest-2/: 24 files
  - api-reference/: 8 files
  - portal/: 1 file
  - legacy/: 3 files

## Git History

- **Initial commit** (79d55de): Original REST 2.0 POC with 27 files
- **Current commit** (793aa2c): Reorganized with rest-2/ subfolder, portal, and legacy sections

## Next Steps

1. Test with `mintlify dev` to verify all navigation paths
2. Deploy to Mintlify dashboard
3. Part 2: Expand API reference with additional REST 1.0 endpoints
4. Part 3: Add APM pages and long-tail content

## Design Principles

- **Clean Navigation**: 3 tabs instead of 6 for simpler UX
- **Logical Grouping**: All REST 2.0 content in one subfolder
- **Link-out Strategy**: Legacy docs provide overview + external links
- **MDX with API Components**: Using Mintlify's ParamField, ResponseField, etc.
