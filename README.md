# Project: **sternsite** – Construction Site Management PWA

## 1. Project Overview
**c10n‑site** is a multi‑tenant Progressive Web Application (PWA) that streamlines construction‑site operations.  
Phase 1 delivers a robust, user‑friendly **time‑tracking** solution for construction companies and their workers.  
The long‑term vision is to evolve into a full‑featured construction‑management platform.

Key characteristics:

- **Multi‑tenant architecture** – multiple companies share one application instance while keeping data isolated and secure.
- **Mobile‑first experience** – workers interact through an installable PWA optimised for field conditions.

---

## 2. Target Audience
| User Group | Primary Needs |
|------------|---------------|
| **Construction Companies** (administrators & managers) | Manage sites, register workers, track and export hours |
| **Construction Workers** (field personnel) | Simple, reliable clock‑in/out and break tracking |

---

## 3. Key Features

### 3.1 Multi‑Tenant Architecture
- Single application instance serves many companies (tenants).  
- Tenant data (sites, users, time records) remains logically separated and secure.  
- Each company has a dedicated administrative view.

### 3.2 Company Administration Portal (Web)
A browser‑based console for company admins.

| Capability | Details |
|------------|---------|
| **Company Registration & Profile** | Sign‑up and manage company details |
| **Construction‑Site Management** | Add, edit, delete sites; store precise latitude/longitude |
| **Worker Management** | Register workers; generate unique registration codes |
| **Time‑Tracking Dashboard** | Real‑time view of clock‑ins, breaks, outs; filters by worker/site/date |
| **Reporting** | Export time records for payroll and project management |

### 3.3 Worker PWA
Mobile‑first PWA for field personnel.

- **Registration** – workers join using the code supplied by their company.  
- **Geolocation & Automatic Site Detection** – GPS suggests the nearest registered site.  
- **Time‑Clock Actions**  
  1. **Start Work**  
  2. **Take Break**  
  3. **Resume Work**  
  4. **End Work**  
  Each action records the exact location stamp.
- **Offline Capability** – records events offline and syncs when connectivity returns.

---

## 4. Proposed Technology Stack
| Layer | Suggested Tech |
|-------|----------------|
| **Frontend** | React or Vue for admin portal & PWA |
| **Backend** | Node.js (Express or NestJS) |
| **Database** | PostgreSQL (relational) *or* MongoDB (NoSQL) with multi‑tenant schema |
| **Geolocation** | Browser Geolocation API |
| **Deployment** | AWS, Google Cloud, or Azure |

---

## 5. Future Enhancements
- Task & project management  
- Equipment and materials tracking  
- Safety & compliance reporting  
- Payroll / accounting integration  
- Advanced analytics & reporting
