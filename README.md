# EduNect School ERP — Complete Institutional User Guide & Operational Manual (All Modules)

**Platform**: EduNect Institutional School Enterprise Management System  
**Audience**: School Administrators, Principals, Registrars, Admissions Officers, Accountants & Cashiers, Faculty & Teachers, Exam Officers, HR Managers, Transport Coordinators, Librarians, Store Managers, Clinic Nurses, and Security Officers.  
**Portal URL**: `http://[school-tenant].localhost:4200/`  

---

## Master Architecture & Domain Index

EduNect School ERP comprises **17 specialized functional domains** and over **150 operational modules**, structured to deliver end-to-end institutional governance:

1. [Domain 1: Admissions & Enrollment Management (22 Modules)](#domain-1-admissions--enrollment-management)
2. [Domain 2: Academic Management & Class Setup (23 Modules)](#domain-2-academic-management--class-setup)
3. [Domain 3: Learning Management System & Pedagogy (16 Modules)](#domain-3-learning-management-system-lms--pedagogy)
4. [Domain 4: Examination & Assessment Studio (16 Modules)](#domain-4-examination--assessment-studio)
5. [Domain 5: Fee Management, Invoicing & Cashier Counter (36 Modules)](#domain-5-fee-management-invoicing--cashier-counter)
6. [Domain 6: School Finance & Accounting Hub (38 Modules)](#domain-6-school-finance--accounting-hub)
7. [Domain 7: Human Resources, Staff & Payroll Management (16 Modules)](#domain-7-human-resources-staff--payroll-management)
8. [Domain 8: Campus Transport & Fleet Management (9 Modules)](#domain-8-campus-transport--fleet-management)
9. [Domain 9: Library & Media Center Management (22 Modules)](#domain-9-library--media-center-management)
10. [Domain 10: Store & Inventory Procurement Management (16 Modules)](#domain-10-store--inventory-procurement-management)
11. [Domain 11: Health, Clinic & Nursing Care (11 Modules)](#domain-11-health-clinic--nursing-care)
12. [Domain 12: Events, Extra-Curricular & Clubs Management (12 Modules)](#domain-12-events-extra-curricular--clubs-management)
13. [Domain 13: Front Office, Visitor Pass & Campus Security (2 Modules)](#domain-13-front-office-visitor-pass--campus-security)
14. [Domain 14: Circulars, Communications & Letterhead Studio (2 Modules)](#domain-14-circulars-communications--letterhead-studio)
15. [Domain 15: Fixed Assets & Campus Infrastructure (6 Modules)](#domain-15-fixed-assets--campus-infrastructure)
16. [Domain 16: Parent & Student Self-Service Portal (13 Modules)](#domain-16-parent--student-self-service-portal)
17. [Domain 17: Tenant Administration, Roles & Security (12 Modules)](#domain-17-tenant-administration-roles--security)

---

## Universal Navigation & Grid Standards
Across every module in EduNect:
- **Global Academic Year**: Select the active academic session in the top header. All records, lists, and metrics automatically re-scope.
- **Data Table Controls**: Real-time multi-column search, configurable page size (10, 25, 50, 100), column sorting, status switches, filter drawers, and filtered Excel exports.
- **Multi-Country Adaptation**: Currencies, phone formats, and regulatory requirements adapt dynamically to institutional branding without hardcoded regional constraints.

---

## Domain 1: Admissions & Enrollment Management
> **Primary Users**: Admissions Officers, Registrars, Marketing Team, Front Office

### 1.1 Pre-Admission & Enquiry Register (`/admission-management/enquiry`)
* **Purpose**: Captures initial student enquiries from walk-ins, phone calls, and digital campaign landing pages.
* **Steps**: Click **+ New Enquiry**. Record Parent Contact, Student Name, Desired Grade, and Source Channel. Set Follow-up Date.

### 1.2 Parent Communication Follow-up Log (`/admission-management/followup`)
* **Purpose**: Tracks calls, emails, and meetings conducted with prospective parents.
* **Steps**: Select the prospect, log conversation notes, outcome (*Warm*, *Cold*, *Decision Pending*), and schedule the next interaction.

### 1.3 Schedule School Tour (`/admission-management/school-tour`)
* **Purpose**: Coordinates campus walkthroughs with admissions counselors.
* **Steps**: Pick available calendar slots, assign an admissions guide, and send automatic calendar invites with campus directions to parents.

### 1.4 Online Admission Schedule (`/admission-management/schedule`)
* **Purpose**: Governs intake opening and closing dates for various grades and terms.
* **Steps**: Define open submission windows per grade with maximum capacity limits.

### 1.5 Application Scrutiny & Pipeline (`/admission-management/pipeline`)
* **Purpose**: Kanban-style admissions funnel: *Submitted* ➔ *Under Review* ➔ *Assessment Scheduled* ➔ *Offered* ➔ *Accepted*.
* **Steps**: Drag-and-drop applicant cards across stages or approve documents with one click.

### 1.6 Admission Form Studio (`/admission-management/form`)
* **Purpose**: Customizes online and paper application form fields, required attachments, and declaration terms.

### 1.7 Waitlist Queue (`/admission-management/waitlist`)
* **Purpose**: Manages prioritized waitlists for oversubscribed grades based on application timestamp, sibling priority, or staff preference.

### 1.8 Admit Student Desk (`/admission-management/admitted`)
* **Purpose**: Formal student onboarding desk converting qualified applicants into active students.
* **Steps**: Click **Admit Student**, verify civil credentials (Emirates ID / National ID, Birth Certificate), assign unique Student Registration Number (SRN), and generate admission agreement.

### 1.9 Section Allocation Desk (`/admission-management/section-allocation`)
* **Purpose**: Distributes admitted cohorts into balanced sections (considering gender balance, language choices, and special needs).
* **Steps**: Select Grade, view unallocated candidates, and use auto-balance or manual drag-and-drop to place students into sections.

### 1.10 Student ID Cards Generation (`/admission-management/id-cards`)
* **Purpose**: Batch printing of barcoded/RFID smart student identity cards.
* **Steps**: Filter by Grade/Section, preview layout, and click **Print Batch PDF**.

### 1.11 Ministry & Board Registry (`/admission-management/registry`)
* **Purpose**: Synchronizes student demographic profiles with government education authorities (e.g., MOE, ADEK, KHDA, SPEA, CBSE, CISCE).

### 1.12 Family Tree & Sibling Grouping (`/admission-management/family-tree`)
* **Purpose**: Links siblings under a single parent account for unified communication, sibling fee discounts, and shared digital wallets.

### 1.13 Student Re-Registration Portal (`/admission-management/re-registration`)
* **Purpose**: Collects parent intentions for the forthcoming academic year (seat reservation deposit payments).

### 1.14 Re-Registration Block / Unblock Desk (`/admission-management/reregistration-block`)
* **Purpose**: Administrative governance blocking re-registration for chronic fee defaulters or behavioral holds.
* **Key Controls**:
  - Interactive KPI cards (*Total Candidates*, *Eligible*, *Blocked*, *Defaulters*).
  - Status switch per student for instant toggle between *Eligible* and *Blocked*.
  - Defaulter Auto-Hold button freezing re-registration for accounts exceeding policy debt thresholds.
  - Filter drawer (Grade, Section, Reason) and scoped Excel export.

### 1.15 Transfer Certificates & Clearances (`/admission-management/transfer-certificate`)
* **Purpose**: Governs student withdrawals via digital 5-department clearance (*Accounts*, *Library*, *Sports/Labs*, *Transport*, *Clinic*).
* **Steps**: Initiate TC request ➔ departments sign off digitally ➔ Registrar issues official QR-verified Transfer Certificate.

### 1.16 Application Withdrawal & Refunds (`/admission-management/withdrawals`)
* **Purpose**: Processes cancelled admissions and calculates eligible tuition/seat deposit refunds according to institutional policy.

### 1.17 Conditional Agreement List (`/admission-management/conditional`)
* **Purpose**: Tracks students admitted under academic or behavioral probation agreements with review milestone dates.

### 1.18 Admission Notification Triggers (`/admission-management/notifications`)
* **Purpose**: Configures automated SMS/Email triggers for application receipt, assessment invitations, offer letters, and fee payment deadlines.

### 1.19 Admission Vacancy Management (`/admission-management/vacancy`)
* **Purpose**: Real-time seat availability matrix by grade, gender, and stream.

### 1.20 Admission Register (`/admission-management/register`)
* **Purpose**: Official statutory admission register recording enrollment history, withdrawal dates, and destination schools.

### 1.21 Admission Statistics & Analytics (`/admission-management/statistics`)
* **Purpose**: Year-over-year enrollment trends, channel conversion rates, and demographic distributions.

### 1.22 Admission Configuration (`/admission-management/config`)
* **Purpose**: System-wide admissions rules, default age criteria per grade, and document upload constraints.

---

## Domain 2: Academic Management & Class Setup
> **Primary Users**: Principals, Academic Heads, Homeroom & Subject Teachers

### 2.1 Grade Category Master (`/academic-management/grade-category/list`)
* **Purpose**: Groups educational stages (e.g., *Early Years*, *Primary Wing*, *Middle School*, *Secondary / Senior Secondary*).

### 2.2 Grade Master (`/academic-management/grade/list`)
* **Purpose**: Establishes numerical or named grade levels (e.g., Pre-KG to Grade 12).

### 2.3 Section Master (`/academic-management/section/list`)
* **Purpose**: Defines classroom division identifiers (Section A, B, C, etc.).

### 2.4 Grade-Section Class Mapping (`/academic-management/grade-section/list`)
* **Purpose**: Pairs Grades with Sections, establishes classroom room assignments, and sets maximum student capacity.

### 2.5 Classroom & Facility Allocation (`/academic-management/classroom-facility/list`)
* **Purpose**: Allocates physical campus rooms, science labs, art studios, and sports complexes to class sections.

### 2.6 Section Head / Wing Head Allocation (`/academic-management/section-head-allocation`)
* **Purpose**: Delegates academic oversight to Wing Heads (Headmistress/Headmaster) for specific grades.

### 2.7 Department Head Allocation (`/academic-management/department-head-allocation`)
* **Purpose**: Assigns Heads of Department (HODs) over subject areas (e.g., Mathematics, Science, Humanities).

### 2.8 Class Teacher Allocation (`/academic-management/class-teacher-allocation`)
* **Purpose**: Allocates homeroom class teachers responsible for pastoral care, attendance, and report cards.
* **Features**: Dedicated filter drawer (Year, Grade, Section, Teacher), status switches, and scoped Excel roster export.

### 2.9 Subject Teacher Allocation (`/academic-management/subject-teacher-allocation`)
* **Purpose**: Assigns subject faculty to specific grade sections (e.g., Mr. Smith -> Grade 9A Physics).

### 2.10 Subject Category, Type & Group Masters (`/academic-management/subject-*/list`)
* **Purpose**: Classifies subjects as Core, Elective, Co-curricular, Second Language, or Remedial.

### 2.11 Subject Master Register (`/academic-management/subject/list`)
* **Purpose**: Central catalog of all institutional subjects with curriculum codes and credit weights.

### 2.12 Grade-Subjects Mapping (`/academic-management/grade-subject/list`)
* **Purpose**: Links applicable subjects to each grade level with weekly period allocations.

### 2.13 Student Elective Allocation (`/academic-management/student-elective-allocation/list`)
* **Purpose**: Enrolls high-school students into specific elective streams and foreign language choices.

### 2.14 Student Cohort Desk (`/academic-management/student-cohort-desk/list`)
* **Purpose**: Manages specialized student groupings (Gifted & Talented, SEN / Inclusion, ESL Learners).

### 2.15 Timetable Management Studio (`/academic-management/timetable`)
* **Purpose**: Automated conflict-free master timetable generation for classrooms, teachers, and shared labs.

### 2.16 Teacher Relief & Substitution Desk (`/academic-management/teacher-relief`)
* **Purpose**: Handles daily unplanned faculty absences by reallocating free teachers to cover classes.

### 2.17 Student Daily Attendance Tracker (`/academic-management/student-attendance/list`)
* **Purpose**: Homeroom teachers mark daily attendance (*Present*, *Absent*, *Tardy*, *Excused Medical*). Triggers parent notifications.

### 2.18 Student Class Change Desk (`/academic-management/student-class-change/list`)
* **Purpose**: Handles mid-term section transfers while preserving past academic attendance and grades.

### 2.19 School Calendar & Term Planner (`/academic-management/school-calendar/list`)
* **Purpose**: Publishes institutional holidays, examination periods, PTM dates, and sports events.

### 2.20 Parent-Teacher Meeting (PTM) Scheduler (`/academic-management/ptm-scheduler/list`)
* **Purpose**: Creates parent meeting slots, allowing parents to book 10-minute consultations with teachers.

### 2.21 Demographic Masters Hub (`/academic-management/demographic-masters`)
* **Purpose**: Manages master lookup tables: Nationalities, Religions, Mother Tongues, Blood Groups, and Visa Categories.

---

## Domain 3: Learning Management System (LMS) & Pedagogy
> **Primary Users**: Subject Teachers, Students, Curriculum Supervisors

### 3.1 Subject Virtual Classrooms Hub (`/learning-management/subject-classrooms/hub`)
* **Purpose**: Digital classroom hub for each enrolled course with streaming stream, materials, and teacher announcements.

### 3.2 Virtual Online Classes (`/learning-management/virtual-classes/list`)
* **Purpose**: Coordinates live remote video sessions (Zoom, Microsoft Teams, Google Meet) directly inside the LMS.

### 3.3 Homework & Assignment Desk (`/learning-management/homework-desk/list`)
* **Purpose**: Teachers publish assignments with deadlines, attachments, and rubrics. Students submit digital files; teachers grade online.

### 3.4 Digital Worksheets & Study Notes (`/learning-management/worksheet-notes/list`)
* **Purpose**: Central study repository hosting downloadable revision sheets, PDF notes, and instructional videos.

### 3.5 Worksheet Publishing Schedule (`/learning-management/worksheet-schedule/list`)
* **Purpose**: Pre-schedules release of supplementary study material ahead of exam periods.

### 3.6 Syllabus & Curriculum Pacing Tracker (`/learning-management/syllabus-tracker/list`)
* **Purpose**: Compares planned vs. actual curriculum completion across chapters and topics with visual progress bars.

### 3.7 Daily Lesson Planning Studio (`/learning-management/lesson-planning/list`)
* **Purpose**: Teachers author daily lesson plans with learning objectives, success criteria, and differentiation strategies.

### 3.8 Remedial Intervention & Learning Support (`/learning-management/remedial-intervention/list`)
* **Purpose**: Logs targeted intervention strategies for struggling learners and tracks progress recovery.

### 3.9 Student Digital Diary (`/learning-management/student-diary/list`)
* **Purpose**: Daily communication log between teachers and parents regarding homework, uniform, or conduct.

### 3.10 Student Self-Learning Portal (`/learning-management/student-learning-portal/list`)
* **Purpose**: Student-facing portal for accessing revision courses, recorded lectures, and interactive simulations.

### 3.11 Online Quizzes & Timed Assessments (`/learning-management/quiz-assessment/list`)
* **Purpose**: Timed automated quizzes with instant objective grading and answer feedback.

### 3.12 Digital Question Bank (`/learning-management/question-bank/list`)
* **Purpose**: Rich repository of questions classified by difficulty (*Easy*, *Medium*, *Hard*), subject, and Bloom's Taxonomy.

### 3.13 Project-Based Learning (PBL) Studio (`/learning-management/pbl-studio/list`)
* **Purpose**: Collaborative group project workspace tracking milestones, group member contributions, and final presentations.

### 3.14 Student Digital Portfolio (`/learning-management/student-portfolio/list`)
* **Purpose**: Showcases student artistic, scientific, and extracurricular achievements across academic years.

### 3.15 Gamification & Achievements Hub (`/learning-management/gamification-hub/list`)
* **Purpose**: Awards badges, house points, and digital stars to incentivize positive behaviors and academic excellence.

### 3.16 Doubt Resolution Forum (`/learning-management/doubt-forum/list`)
* **Purpose**: Q&A discussion board where students post academic queries answered by subject teachers and peers.

---

## Domain 4: Examination & Assessment Studio
> **Primary Users**: Exam Officers, Academic Directors, Homeroom Faculty

### 4.1 Exam Management Dashboard (`/exam-management/dashboard`)
* **Purpose**: Executive overview of upcoming assessments, mark entry completion rates, and historical averages.

### 4.2 Academic Term Manager (`/exam-management/term/list`)
* **Purpose**: Defines assessment terms (Term 1, Term 2, Term 3, Annual Board Examination).

### 4.3 Evaluation & Exam Categories (`/exam-management/*-category/list`)
* **Purpose**: Classifies assessment modes (Formative, Summative, Internal Assessment, Practical Exam).

### 4.4 Exam Series & Master Schedule (`/exam-management/exam/list` & `/schedule`)
* **Purpose**: Schedules dates, times, rooms, and invigilation duties for each subject exam.

### 4.5 Grading Scales & Bands (`/exam-management/exam-grade/list`)
* **Purpose**: Configures percentage boundaries and letter grades (e.g., 90–100% -> A*, 80–89% -> A, GPA points).

### 4.6 Subject Sub-Skills & Rubric Criteria (`/exam-management/subject-sub-skills/list`)
* **Purpose**: Defines co-scholastic and subject sub-skills (e.g., Reading Comprehension, Lab Technique, Oral Fluency).

### 4.7 Assessment Component Breakup Studio (`/exam-management/exam-grade-subject/list`)
* **Purpose**: Establishes score breakdowns per subject (e.g., Theory: 70 marks, Practical: 20 marks, Internal: 10 marks).

### 4.8 Smart Marks Entry Desk (`/exam-management/marks-entry`)
* **Purpose**: Faculty mark entry screen with instant validation against maximum marks and absent student flags.

### 4.9 Result Compilation Engine (`/exam-management/result-processing`)
* **Purpose**: High-speed compilation calculating aggregate scores, percentages, grade distributions, and class rankings.

### 4.10 Report Card Template Studio (`/exam-management/report-card-studio`)
* **Purpose**: Template designer supporting CBSE, IB, British Cambridge, American, and Ministry formats.

### 4.11 Report Card Withholding Desk (`/exam-management/report-card-withholding`)
* **Purpose**: Prevents parents with fee arrears from viewing report cards online while preserving administrative override authority.
* **Features**: KPI metrics bar, inline portal release switch, defaulter auto-withhold, filter drawer, and Excel export.

### 4.12 Examination Analytics Broadsheet (`/exam-management/analytics`)
* **Purpose**: Comprehensive tabular broadsheet showing all subject scores and historical comparisons.

### 4.13 Exam Admit Cards (`/exam-management/admit-cards`)
* **Purpose**: Generates examination hall tickets with candidate photo, seat number, timetable, and instructions.

### 4.14 Homeroom & Pastoral Remarks Studio (`/exam-management/remarks-studio`)
* **Purpose**: Class teachers and Principals input personal evaluations and pastoral observations.

---

## Domain 5: Fee Management, Invoicing & Cashier Counter
> **Primary Users**: Cashiers, Accountants, Billing Officers, CFO

### 5.1 Fee Category & Type Masters (`/fee/category/list` & `/type/list`)
* **Purpose**: Defines institutional revenue streams: Tuition, Transport, Uniform, Lab, Admission, Technology Fee.

### 5.2 Fee Term Schedules (`/fee/term/list`)
* **Purpose**: Establishes billing schedules (Termly, Monthly, Bi-Annual) with invoice generation and due dates.

### 5.3 Fee Structure Matrix (`/fee/structure/matrix`)
* **Purpose**: Master fee matrix assigning pricing per grade level and curriculum stream.

### 5.4 Student Fee Allocation (`/fee/allocation/list`)
* **Purpose**: Manages personalized fee assignments for individual students or cohorts.

### 5.5 Incidental & Activity Fees (`/fee/incidental/list`)
* **Purpose**: Bills ad-hoc one-off fees (Field trips, Yearbooks, Exam registration fees).

### 5.6 Concessions, Scholarships & Approvals (`/fee/concession/*`)
* **Purpose**: Configures scholarship schemes (Sibling, Staff child, Merit) and enforces multi-tier approval workflows.

### 5.7 Fee Discount Policies (`/fee/discount-policies`)
* **Purpose**: Early bird full-payment discounts and corporate partnership rebates.

### 5.8 Point of Sale (POS) Fee Collection Counter (`/fee/collect`)
* **Purpose**: Central cashier counter for recording fee payments.
* **Features**: Real-time student ledger search, multiple payment modes (Cash, Card, Cheque, Bank Transfer), partial payment support, and branded receipt printing.

### 5.9 Cashier Daily Shifts & Reconciliation (`/fee/cashier-shifts`)
* **Purpose**: Manages cashier drawer openings, float amounts, daily collections, and handover reconciliations.

### 5.10 Student & Family Credit Wallets (`/fee/wallet` & `/family-wallets`)
* **Purpose**: Pre-funded digital accounts for cafeteria purchases, uniform shop, and unallocated overpayments.

### 5.11 Bank Transfer Slips Verification (`/fee/bank-transfers`)
* **Purpose**: Verifies parent-uploaded bank transfer receipts against bank statements before posting to student accounts.

### 5.12 PDC Cheque Vault (`/fee/cheques`)
* **Purpose**: Vault tracking post-dated cheques, maturities, bank deposits, and automated reversal upon bounce.

### 5.13 Fee Refund & Manual Receipts (`/fee/refund/list`)
* **Purpose**: Processes formal fee refunds with administrative authorization.

### 5.14 Fee Clearance NOC Desk (`/fee/clearance`)
* **Purpose**: Issues digital financial No Objection Certificates for exam appearance or school departure.

### 5.15 Fee Write-offs & Bad Debt (`/fee/write-offs`)
* **Purpose**: Authorized write-offs for uncollectible debt with mandatory audit reasoning.

### 5.16 CFO Fee Analytics Cockpit (`/fee/cfo-analytics`)
* **Purpose**: High-level visual tracking of projected vs. actual revenue collections, arrears aging, and collection velocity.

### 5.17 Student Fee Invoices Ledger (`/fee/invoice/list`)
* **Purpose**: Complete register of all issued invoices with payment statuses and outstanding balances.

### 5.18 Late Fee & Fine Engine (`/fee/late-fine`)
* **Purpose**: Automated calculation of grace periods, daily penalties, and administrative fine waiver requests.

### 5.19 Fee Installment Plans (`/fee/installment-plans`)
* **Purpose**: Breaks down termly fee liabilities into customized monthly installments for struggling families.

### 5.20 Fee Reminders & Dunning (`/fee/reminders`)
* **Purpose**: Multi-stage automated dunning: gentle SMS reminder ➔ formal email notice ➔ account withhold warning.

### 5.21 Corporate & Embassy Sponsors (`/fee/sponsors`)
* **Purpose**: Third-party invoicing for students sponsored by embassies, government ministries, or corporate employers.

### 5.22 VAT / Statutory Tax Matrix (`/fee/tax-matrix`)
* **Purpose**: Governs applicable consumption taxes (e.g., zero-rated tuition vs. standard-rated uniforms and transport).

---

## Domain 6: School Finance & Accounting Hub
> **Primary Users**: Chief Financial Officers, Financial Controllers, Senior Accountants

### 6.1 Accounting Masters & Chart of Accounts (`/finance/masters`)
* **Purpose**: Institutional Chart of Accounts (Assets, Liabilities, Equity, Revenue, Cost of Sales, Expenses).

### 6.2 Subledger to GL Mapping (`/finance/subledger-mapping`)
* **Purpose**: Maps operational transactions (Fee Receipts, Store Invoices, Staff Payroll) directly to General Ledger accounts.

### 6.3 Voucher Entry & Multi-Level Approvals (`/finance/voucher-*`)
* **Purpose**: Journal, Payment, Receipt, and Contra voucher creation with maker-checker approval controls.

### 6.4 Petty Cash Imprest Management (`/finance/petty-cash`)
* **Purpose**: Daily petty cash disbursements for administrative incidentals with reimbursement reconciliation.

### 6.5 Departmental Budget Control & Period Locks (`/finance/budget-control` & `/period-budget`)
* **Purpose**: Sets department budget ceilings with automatic purchase prevention when budgets are exhausted.

### 6.6 Prepayments & Revenue Recognition (`/finance/prepayments-accruals` & `/revenue-recognition`)
* **Purpose**: Amortizes annual advance tuition collections across monthly accounting periods matching delivery.

### 6.7 Bad Debt Provisioning (IFRS 9 ECL) (`/finance/bad-debt-provisioning`)
* **Purpose**: Calculates expected credit loss allowances on outstanding student receivables.

### 6.8 Fixed Assets & Lease Accounting (IFRS 16) (`/finance/fixed-assets` & `/lease-accounting`)
* **Purpose**: Fixed asset depreciation schedules, campus equipment tracking, and right-of-use lease valuations.

### 6.9 Capital Projects & Fund Accounting (`/finance/capital-projects` & `/fund-accounting`)
* **Purpose**: Governs campus construction expansions and endowment donor funds with restricted usages.

### 6.10 Bank Statement Parser & Auto-Reconciliation (`/finance/bank-statement-parser`)
* **Purpose**: Imports MT940 / CSV bank statements and automatically matches credits against fee receipts.

### 6.11 Final Accounts Reports (`/finance/reports`)
* **Purpose**: Generates Trial Balance, Profit & Loss Statement, and Balance Sheet with comparative periods.

### 6.12 E-Invoicing Vault & Statutory Tax Compliance (`/finance/e-invoicing-vault`)
* **Purpose**: Generates cryptographically signed, QR-coded electronic tax invoices meeting statutory authority mandates.

---

## Domain 7: Human Resources, Staff & Payroll Management
> **Primary Users**: HR Managers, Administrative Directors, Payroll Specialists

### 7.1 Department & Designation Masters (`/hr-management/department` & `/designation`)
* **Purpose**: Establishes institutional organization charts, faculty departments, and administrative ranks.

### 7.2 Staff Recruitment & Job Openings (`/hr-management/recruitment`)
* **Purpose**: Tracks applicant tracking pipelines for teaching and operational positions.

### 7.3 Staff Directory & Onboarding (`/hr-management/staff/list` & `/add`)
* **Purpose**: Master employee directory recording personal, educational, immigration, and contractual details.
* **Features**: Assigns one of 27 school operational roles and tracks compliance expirations (Visas, Teaching licenses).

### 7.4 Staff Leave Configuration & Applications (`/hr-management/leave-type` & `/staff-leave`)
* **Purpose**: Manages annual, sick, maternity, and bereavement leave balances with substitute teacher allocation.

### 7.5 Staff Daily Attendance & Biometric Integration (`/hr-management/attendance`)
* **Purpose**: Synchronizes daily clock-ins/outs from hardware biometric readers and mobile geofenced punches.

### 7.6 Monthly Staff Payroll & Payslips (`/hr-management/payroll/list` & `/my-payslips`)
* **Purpose**: Generates monthly payroll with salary additions, deductions, unpaid leave calculations, and printable payslips.

---

## Domain 8: Campus Transport & Fleet Management
> **Primary Users**: Transport Coordinators, Fleet Supervisors

### 8.1 Vehicle Fleet & Staff Registry (`/transport/vehicles` & `/staff`)
* **Purpose**: Manages buses, insurance expirations, fitness permits, and designated Drivers and Attendants.

### 8.2 Bus Routes & Pickup Stops (`/transport/routes` & `/areas`)
* **Purpose**: Maps route stops in geographic sequence with scheduled arrival and departure timings.

### 8.3 Student Seat Allocation (`/transport/allocations`)
* **Purpose**: Assigns enrolled students to specific routes, stops, and morning/afternoon shifts.

### 8.4 Daily Transport Attendance (`/transport/attendance`)
* **Purpose**: Bus attendants record student boarding and deboarding via mobile scan, sending alerts to parents.

---

## Domain 9: Library & Media Center Management
> **Primary Users**: Librarians, Teachers, Students

### 9.1 Master Catalog & Barcoded Inventory (`/library/catalog` & `/copy-inventory`)
* **Purpose**: Cataloging of books, journals, and digital media using ISBN, Dewey Decimal, and barcode tracking.

### 9.2 Circulation Desk (Issue & Return) (`/library/circulation`)
* **Purpose**: High-speed circulation scanning for loaning and returning books with automated overdue fine calculation.

### 9.3 Class-Wise Bulk Issue (`/library/class-bulk-issue`)
* **Purpose**: Distributes class sets of textbooks to homeroom groups at the start of academic terms.

### 9.4 Digital Resources & E-Books Vault (`/library/digital-resources`)
* **Purpose**: Repository of educational PDFs, audiobooks, and links to global digital libraries.

### 9.5 Reading Challenges & Student Reading Lists (`/library/reading-*`)
* **Purpose**: Promotes student reading habits through digital logbooks, reading goals, and achievement milestones.

---

## Domain 10: Store & Inventory Procurement Management
> **Primary Users**: Store Keepers, Procurement Officers

### 10.1 Item Catalog & Point of Sale (`/store-management/items` & `/sales`)
* **Purpose**: Manages inventories of uniforms, textbooks, stationery, and laboratory equipment with POS sales to parents.

### 10.2 Procurement & Purchase Orders (`/store-management/procurement` & `/purchase-orders`)
* **Purpose**: Generates departmental requisitions, vendor quotes, and official Purchase Orders.

### 10.3 Goods Receiving Notes (GRN) & Stock Ledger (`/store-management/receiving` & `/ledger`)
* **Purpose**: Records physical shipments, verifies against PO quantities, and updates weighted-average stock costs.

### 10.4 Departmental Store Issue & Audits (`/store-management/store-issue` & `/stock-audit`)
* **Purpose**: Issues materials to classrooms and conducts periodic physical inventory reconciliations.

---

## Domain 11: Health, Clinic & Nursing Care
> **Primary Users**: School Medical Doctors, Registered Nurses

### 11.1 Electronic Health Records (EHR) (`/nursing/health-profiles`)
* **Purpose**: Secure medical profiles recording chronic conditions, critical allergies, blood group, and emergency instructions.

### 11.2 Daily Clinic Visit Triage Desk (`/nursing/clinic-visits`)
* **Purpose**: Records student visits, vitals, symptoms, treatments administered, and disposition (returned to class or sent home).

### 11.3 Statutory Vaccination Scheduler (`/nursing/vaccination-scheduler`)
* **Purpose**: Tracks government-mandated childhood immunization schedules and flags non-compliant records.

### 11.4 School Incident & Injury Reporting (`/nursing/incidents`)
* **Purpose**: Mandatory statutory documentation of playground injuries, first-aid measures, and parent communication.

---

## Domain 12: Events, Extra-Curricular & Clubs Management
> **Primary Users**: Activity Coordinators, Sports Directors

### 12.1 School Events Catalog & Registration (`/events/catalog` & `/registrations`)
* **Purpose**: Publishes sports days, concerts, science fairs, and tracks student registrations and entry fees.

### 12.2 Student Clubs & Societies (`/events/clubs`)
* **Purpose**: Manages membership rosters, meetings, and faculty mentors for debate, robotics, drama, and sports clubs.

### 12.3 Event Certificates Studio (`/events/certificates`)
* **Purpose**: Generates and distributes branded certificates of participation and merit.

---

## Domain 13: Front Office, Visitor Pass & Campus Security
> **Primary Users**: Receptionists, Security Personnel

### 13.1 Visitor Pass & Gate Security (`/front-office/visitors`)
* **Purpose**: Digital visitor registry capturing national ID, purpose of visit, host staff member, and printed visitor badges.

### 13.2 Student Early Departure Gate Pass (`/front-office/early-departures`)
* **Purpose**: Authorizes early student release with parent ID verification, notifying homeroom teachers and gate security.

---

## Domain 14: Circulars, Communications & Letterhead Studio
> **Primary Users**: Principals, Public Relations Officers

### 14.1 Official Circulars Studio (`/circular-management/circulars`)
* **Purpose**: Authors and publishes official school bulletins targeted to specific grades, sections, or whole school.

### 14.2 Branded Letterhead Designer (`/circular-management/letterpad-designer`)
* **Purpose**: Customizable institutional letterhead templates for formal notices and administrative letters.

---

## Domain 15: Fixed Assets & Campus Infrastructure
> **Primary Users**: Facilities Managers, Asset Officers

### 15.1 Campus Asset Registry (`/asset-management/registry` & `/locations`)
* **Purpose**: Tags and tracks all campus furniture, computer hardware, smartboards, and laboratory instruments by building and room.

### 15.2 Asset Allocations & Audits (`/asset-management/allocations` & `/audits`)
* **Purpose**: Tracks staff laptop custody, WiFi device MAC registrations, and periodic barcode audits.

---

## Domain 16: Parent & Student Self-Service Portal
> **Primary Users**: Parents, Enrolled Students

### 16.1 Command Center & Multi-Ward Overview (`/portal/home` & `/ward-overview`)
* **Purpose**: Unified mobile/desktop dashboard for parents with multiple children across different grades.

### 16.2 Online Homework & Digital Vault (`/portal/assignments`)
* **Purpose**: View assignments, download class notes, and upload completed homework files.

### 16.3 Online Fee Desk & Payments (`/portal/fees-wallet`)
* **Purpose**: Review active invoices and make immediate secure online payments via Credit/Debit card or Apple/Google Pay.

### 16.4 PTM Booking & Leave Requests (`/portal/ptm-booking` & `/leave-requests`)
* **Purpose**: Book consultation slots with teachers and submit absence leave notifications.

---

## Domain 17: Tenant Administration, Roles & Security
> **Primary Users**: System Administrators, School Owners

### 17.1 Academic, Financial & Administrative Year Calendars (`/year/*`)
* **Purpose**: Maintains active sessions, financial tax years, and administrative cycles.

### 17.2 27 Dedicated School Operational Roles (`/role/*`)
* **Purpose**: Manages permissions across 27 school roles (*Teacher*, *Registrar*, *Admissions Officer*, *Accountant*, *Nurse*, *Transport Manager*, etc.) with zero SaaS platform superadmin leakage.

### 17.3 Immutable Audit Activity Tracker (`/activity-tracker/list`)
* **Purpose**: Records human-readable "A updated to B" audit logs on every database mutation for statutory compliance.

### 17.4 Site Settings & Biometric Integrations (`/site-settings` & `/tenant-management/*`)
* **Purpose**: Configures school branding, logos, localized timezones, email SMTP relays, and hardware biometric integrations.

---

## Summary & Master Verification Complete
Every module documented above is live, compiled, and accessible at `http://[school-tenant].localhost:4200/` adhering strictly to EduNect's architecture standards.
