# Product Requirements Document (PRD)

## Product Name: KidTrack Core

---

## Goal  
To reduce mental overload and decision anxiety in child health management by enabling parents to log key health events, receive simple symptom guidance, and share responsibility through a co-parenting-friendly interface.

---

## Problem Statement  
Parents—especially mothers—carry the mental and operational burden of tracking symptoms, doctor visits, school health forms, and treatment routines. They're often uncertain about what symptoms matter, forget key health moments, and struggle to get co-parents equally involved. Existing tools are fragmented, overcomplicated, or not designed for shared use.

---

## MVP Objective  
Deliver a shared, smart health timeline and lightweight symptom guidance assistant in a mobile-first experience that both parents can use. The solution should be usable without training and installable in under 2 minutes.

---

## Target Users  
- **Primary**: Parents (especially moms) of kids aged 2–10 managing everyday child health  
- **Secondary**: Co-parents (spouses, partners) who are less engaged in tracking/logging  

---

## Key Features and Requirements  

### 1. Health Timeline  
- Add entries for: Symptom, Medication, Note  
- Quick-tag entries (e.g., "fever", "rash", "doctor visit")  
- Show timestamp and attribution (e.g., "Logged by Alex at 9:34am")  
- Filter by tag or date  
- Editable/deletable by entry creator  

### 2. Triage Companion  
- Symptom input flow: Fever, Cough, Sleep, Appetite  
- Decision outcomes:
  - Monitor at home  
  - Call pediatrician  
  - Seek urgent care  
- Based on pre-set rule logic (from CDC/AAP)  
- Add result to timeline with one tap  

### 3. Co-Parent Sync  
- Invite second caregiver via email or magic link  
- Shared access to child timeline and entries  
- Track contributor on each log  
- Optional nudge: "You haven't logged in 3+ days"  

---

## Out of Scope (for MVP)  
- AI-driven diagnosis  
- Chat with doctor or school nurse  
- Wearable/device integrations  
- PDF export or data analytics  

---

## UX Requirements  
- Mobile-first responsive design  
- Onboarding should prompt caregiver invite  
- Use gender-neutral, inclusive language  
- Minimalist layout: max 2 clicks to log an event  
- All major actions accessible within 5 seconds  

---

## Tech Stack (Recommended)  
- **Frontend**: React or Flutter  
- **Backend**: Firebase or Supabase  
- **Authentication**: Firebase Auth or magic link  
- **Storage**: Firestore or Supabase tables  
- **Notifications**: In-app, with email optional  

---

## Success Metrics  

| Objective                | KPI                                 | Target       |
|--------------------------|--------------------------------------|--------------|
| Parent engagement        | % logging an event in Week 1        | ≥ 70%        |
| Shared use               | % inviting co-parent                | ≥ 60%        |
| Decision support usage   | % using Triage feature              | ≥ 50%        |
| Co-parent contribution   | % of logs by 2nd caregiver          | ≥ 30%        |
| Retention                | Weekly active users by Week 3       | ≥ 40%        |

---

## Timeline & Milestones (2–4 Weeks)

| Week | Milestone                                  |
|------|--------------------------------------------|
| 1    | Timeline logging UI and backend setup      |
| 2    | Triage logic implementation                |
| 3    | Co-parent onboarding and sync features     |
| 4    | QA, polish, and soft launch                |

---

## Future Considerations (Post-MVP)  
- PDF export for pediatricians or schools  
- Pattern detection (e.g., recurring symptom history)  
- Task assignment between caregivers  
- Additional caregiver roles (e.g., nurse, nanny)  
- Gamified participation or caregiver streaks  
