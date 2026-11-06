# CarePulse — Hospital & Patient Management System (PMS)

A modern, responsive, multi-page web application for hospital clinics and medical practices to manage patients, appointments, electronic health records (EHR), clinical vitals, billing & insurance claims, and medical staff directories.

---

## 🌟 Key Features

- **Multi-Page Interlinked Architecture**: Complete navigation bar across all 7 pages with active link indication, mobile drawer menu, and notification popovers.
- **Centralized Data Store (`store.js`)**: Real-time synchronization across all pages via browser `localStorage` with built-in rich demo seed data (patients, doctors, appointments, invoices, lab reports).
- **Interactive Modals & Workflows**:
  - Register new patient with full clinical validation.
  - Schedule consultations with doctor assignment & slot picker.
  - Issue official digital prescriptions (Rx) with auto-signing.
  - Create itemized hospital billing statements with 85/15 insurance adjudication.
  - Live vital signs editor (Blood Pressure, Heart Rate, SpO2, Temperature).
- **Printable Medical Summaries**: Dedicated print styles for Patient EHR summaries, official Rx pads, and itemized billing receipts (`window.print()`).

---

## 📑 Page Directory & Linking Structure

| Page | File | Purpose & Key Features |
|---|---|---|
| **Dashboard** | [`index.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/index.html) | Hospital operational metrics, inpatient occupancy rate, daily visits, recent admissions, doctor shift radar, quick action triggers. |
| **Patients Directory** | [`patients.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/patients.html) | Patient search by name/ID/phone/blood group, department & admission status filters, "Register Patient" modal, individual EHR links. |
| **Patient EHR Profile** | [`patient-details.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/patient-details.html) | Comprehensive patient dossier with tabbed views: Vitals tracker, chronic conditions & severe allergy warnings, active medications, lab diagnostics, encounter timeline, and follow-up booking. |
| **Consultation Scheduler** | [`appointments.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/appointments.html) | Calendar & queue manager, filter by status (Scheduled / In Consultation / Completed), book new appointment modal with pre-selection support. |
| **EHR & Lab Records** | [`records.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/records.html) | Central laboratory & pathology repository (CBC, ECG, MRI, X-ray), digital prescription generator with printable Rx pad. |
| **Billing & Claims** | [`billing.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/billing.html) | Revenue tracking, insurance claims with major carriers (BlueCross, Aetna, Cigna, UnitedHealthcare), invoice generator, printable itemized receipt modal. |
| **Doctors & Medical Staff** | [`doctors.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/doctors.html) | Specialist directory across Cardiology, Neurology, Pediatrics, Orthopedics, Internal Medicine, and Dermatology; live shift and availability status. |

---

## 📂 Project Directory Structure

```text
patient-management-system/
├── index.html              # Hospital Overview & Operational Dashboard
├── patients.html           # Master Patient Directory & Registration
├── patient-details.html    # Detailed EHR Dossier, Vitals & Treatment Log
├── appointments.html       # Consultation Queue & Slot Scheduling
├── records.html            # Lab Diagnostics Archive & Digital Rx Generator
├── billing.html            # Hospital Invoices & Insurance Claims
├── doctors.html            # Medical Specialists & Staff Roster
├── css/
│   └── styles.css          # Badges, transitions, custom scrollbars, print stylesheet
├── js/
│   ├── store.js            # Unified state management, mock database, localStorage API
│   └── main.js             # UI controls, active navbar, toast alerts, notification popover
└── README.md               # Documentation & Guide
```

---

## 🚀 How to Run

1. Open any browser (Chrome, Edge, Firefox, Safari).
2. Double-click or open [`index.html`](file:///C:/Users/manoj/.gemini/antigravity/scratch/patient-management-system/index.html).
3. Alternatively, serve with any local HTTP server (such as Python, Live Server, or Node `npx serve`):
   ```powershell
   cd C:\Users\manoj\.gemini\antigravity\scratch\patient-management-system
   python -m http.server 3000
   ```
4. Access at `http://localhost:3000`.
