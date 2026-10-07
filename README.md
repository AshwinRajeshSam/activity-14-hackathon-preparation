# Activity 14: Hackathon Preparation & Problem Scoping

**Course:** Portfolio Building (B25CS0311) — 3rd Semester B.Tech CSE, REVA University  
**Team Name:** DevSphere  
**Project Concept:** CampusHub — Smart Lost & Found and Peer Resource Exchange  

---

## 1. Executive Summary
This repository captures the complete preparation, team formation, hackathon shortlisting, ideation scoring, and scoped technical architecture developed during Activity 14. This groundwork establishes the blueprint for the upcoming hackathon development sprint.

---

## 2. Team Roster & Complementary Roles (Section 1)

| Member Name | Degree & Semester | Primary Hackathon Role | Core Strengths & Responsibilities |
| :--- | :--- | :--- | :--- |
| **Ashwin Rajesh Sam** *(Team Lead)* | B.Tech CSE (3rd Sem) | Backend & Cloud Architect | System architecture, REST API design, Firebase/PostgreSQL integration, and cloud deployment pipelines. |
| **Rohan Sharma** | B.Tech CSE (3rd Sem) | Frontend & Client Engineer | React/Next.js component development, responsive UI state management, and API consumption. |
| **Ananya Rao** | B.Tech CSE (3rd Sem) | UI/UX Designer & Product Lead | User flow wireframing in Figma, pitch deck preparation, accessibility compliance, and product demo presentation. |

---

## 3. Shortlisted Hackathon (Section 2)
- **Event Name:** **Smart India Hackathon (SIH) — Student Campus Innovation Sprint**
- **Hosting Platform:** Unstop & Devfolio
- **Platform Direct Link:** [https://unstop.com/hackathons/smart-india-hackathon-campus-edition](https://unstop.com/hackathons/smart-india-hackathon-campus-edition)
- **Mode:** Hybrid (Online initial qualifiers, 36-hour offline grand finale)
- **Team Size Constraints:** 3–4 members
- **Registration Deadline:** November 15, 2026
- **Submission Requirements:** 
  1. Live deployed web application prototype.
  2. Public GitHub repository with clean commit history.
  3. 3-minute video pitch highlighting social impact and technical scalability.

---

## 4. Problem Statement Ideation & Filtering Matrix (Section 3)

Ideas were evaluated on a scale of 1 to 5 across **Feasibility** (can our team ship a working prototype within 36 hours using familiar tools) and **Impact** (does it solve a widespread, painful real-world problem for users):

| Idea # | Problem Concept | Feasibility (1-5) | Impact (1-5) | Composite Score | Selection Decision |
| :-: | :--- | :-: | :-: | :-: | :--- |
| **1** | **CampusHub: Hostel Lost & Found + Resource Exchange** | **5 / 5** | **5 / 5** | **10 / 10** | **SELECTED** |
| 2 | Automated Smart Attendance via Bluetooth Low Energy (BLE) | 3 / 5 | 4 / 5 | 7 / 10 | Deprioritized due to hardware dependency risks |
| 3 | AI-Driven Campus Canteen Queue Predictor & Food Pre-Order | 4 / 5 | 3 / 5 | 7 / 10 | Deprioritized due to vendor POS integration barriers |

### Selection Justification:
Idea 1 provides the optimal balance of immediate social impact within campus hostels, zero hardware dependencies, and a clean technical scope that our team can execute to completion with polished UX and authenticated database operations.

---

## 5. Scoped Problem Statement & Technical Architecture (Section 4)

### Problem Statement Paragraph:
> *Hostel students frequently lose personal items (calculators, chargers, ID cards, water bottles) with no central, searchable medium to report or recover them, relying instead on chaotic, ephemeral WhatsApp groups where critical notices get buried within minutes. CampusHub is a centralized web platform where campus residents can securely report found items with photos, tag specific hostel blocks and timestamps, and search for lost belongings using intelligent category and location filters. By incorporating authenticated institutional email sign-ins and an integrated peer exchange board for semester textbook handovers, CampusHub drastically minimizes property loss and promotes circular reuse across university dormitories.*

### Technical Architecture & Tech Stack:
- **Client Tier (Frontend):**
  - Framework: React.js (Vite) with Tailwind CSS for rapid responsive design.
  - State Management: React Context / Zustand for lightweight reactive state.
  - Icons & Typography: Lucide React and Inter typography.
- **Service Tier (Backend / Auth / DB):**
  - Authentication: Firebase Authentication with institutional Google OAuth (`@reva.edu.in` domain restriction).
  - Database: Cloud Firestore for real-time document sync, compound querying by hostel block, and sub-second retrieval.
  - Storage: Cloud Storage for item verification image uploads.
- **Deployment & CI/CD:**
  - Client Deployment: Vercel with automatic pull-request preview environments.
  - Version Control: GitHub organization repository with protected main branch and peer review PR rules.

---

## 6. Deliverables & Evidence Checklist
- [x] Team roster finalized with 3 members and complementary skill assignments
- [x] Real hackathon shortlisted with verified registration deadlines and platform links
- [x] 3 distinct problem statement ideas evaluated with Feasibility vs Impact matrix
- [x] Scoped problem statement paragraph and end-to-end tech stack documented
- [x] Repository shared with all team members for immediate build-phase kick-off
