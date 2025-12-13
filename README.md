# 97k-database - Shared Module of super-brain-digital-twin

> **MAIN PROJECT:** [super-brain-digital-twin v5.0 (97v.ru)](https://github.com/vik9541/super-brain-digital-twin)  
> **MASTER DOC:** [MASTER_README.md](https://github.com/vik9541/super-brain-digital-twin/blob/main/MASTER_README.md)  
> **ARCHITECTURE:** [STRUCTURE.md](https://github.com/vik9541/super-brain-digital-twin/blob/main/STRUCTURE.md)

---

## This Module: PostgreSQL Database Schema

- Status: PHASE 12 SYNCED
- Stack: PostgreSQL 15 + Prisma ORM
- Type: Shared database (all 97k modules connect here)
- Provider: Supabase

## Schema Source of Truth

**MASTER**: 97k-backend/prisma/schema.prisma  
**REPLICA**: 97k-database/prisma/schema.prisma (synced from backend)

## Tables (17+)

- User (authentication and profiles)
- Product (catalog items)
- Order (order management)
- AppleContact, AppleContactSync (iOS - PHASE 10)
- GoogleContact, GoogleContactSync (Android - PHASE 11)
- OutlookContact, OutlookContactSync (Web - PHASE 12)
- Analytics (event tracking)
- GDPRLog (privacy audit)

## Related Modules

- [super-brain-digital-twin](https://github.com/vik9541/super-brain-digital-twin) - Main Project
- [97k-backend](https://github.com/vik9541/97k-backend) - NestJS API (source of schema)
- [97k-frontend](https://github.com/vik9541/97k-frontend) - React app
- [97k-infrastructure](https://github.com/vik9541/97k-infrastructure) - Deployment
- [97k-n8n-workflows](https://github.com/vik9541/97k-n8n-workflows) - Automation
- [97k-97v-specs](https://github.com/vik9541/97k-97v-specs) - Specs

---

**Status**: SYNCED | **Type**: PostgreSQL Database | **Module of**: super-brain-digital-twin v5.0
