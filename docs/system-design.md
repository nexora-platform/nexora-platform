# System Design

This document explains the internal design decisions behind the Nexora Platform.

## Design Goals

- Scalability
- Tenant isolation
- Secure authentication
- Independent service deployment

## Multi-Tenant Strategy

The platform uses a shared database strategy with tenant isolation.

Each entity includes a tenantId to ensure data separation between tenants.