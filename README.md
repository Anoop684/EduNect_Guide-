# EduNect School ERP — Master User Guide & Operational Manual

**Platform**: EduNect Institutional School Enterprise Management System  
**Audience**: School Administrators, Principals, Registrars, Admissions Officers, Accountants & Cashiers, Teachers & Faculty, Exam Officers, HR Managers, Transport Coordinators, and Clinic Staff.  
**Portal**: `http://[school-tenant].localhost:4200/`  

---

## Table of Contents
1. [System Navigation & Role-Based Access](#1-system-navigation--role-based-access)
2. [Module 1: Academic Foundation & Setup](#module-1-academic-foundation--setup)
3. [Module 2: Admissions & Student Lifecycle Management](#module-2-admissions--student-lifecycle-management)
4. [Module 3: Fee Management, Invoicing & Cashier Desk](#module-3-fee-management-invoicing--cashier-desk)
5. [Module 4: Learning Management System (LMS) & Curriculum](#module-4-learning-management-system-lms--curriculum)
6. [Module 5: Examination Studio, Grading & Report Card Release](#module-5-examination-studio-grading--report-card-release)
7. [Module 6: Campus Transport & Fleet Operations](#module-6-campus-transport--fleet-operations)
8. [Module 7: Human Resources, Staff & Payroll Management](#module-7-human-resources-staff--payroll-management)
9. [Module 8: Clinic & Student Health Management](#module-8-clinic--student-health-management)
10. [Module 9: School Finance & Accounting Hub](#module-9-school-finance--accounting-hub)
11. [Module 10: Parent & Student Self-Service Portal](#module-10-parent--student-self-service-portal)

---

## 1. System Navigation & Role-Based Access

### 1.1 Logging In
1. Open your school's dedicated URL (e.g., `http://sisad.localhost:4200/`).
2. Enter your assigned school email and password.
3. Click **Sign In**.
4. The system validates your credentials and loads the appropriate dashboard based on your assigned institutional role (e.g., Tenant Admin, Principal, Teacher, Cashier).

### 1.2 Global Academic Year Switcher
- Located in the top navigation header.
- Automatically selects the current active academic year.
- Switching the academic year refreshes all data tables, KPI metrics, student lists, and fee ledgers to display records for that specific academic year.

### 1.3 Universal Data Table Controls
Every data grid in EduNect provides standard tools:
- **Search Bar**: Real-time multi-column search filtering.
- **Entries per Page**: Toggle between 10, 25, 50, or 100 rows.
- **Column Sorting**: Click any column header to sort ascending or descending.
- **Status Switches**: Click the toggle switch to immediately activate or deactivate an item.
- **Filter Drawer**: Click the filter icon to apply multi-criteria filtering (Grade, Section, Status, Date Range).
- **Excel Export**: Click **Export** to download the currently filtered view directly to an `.xlsx` file.

---

## Module 1: Academic Foundation & Setup
> **Primary Users**: School Administrators, Principals, Academic Coordinators

### 1.1 Academic Year Setup
* **Navigation**: `Academic Management` > `Academic Year`
* **Purpose**: Defines the school calendar sessions.
* **Step-by-Step Instructions**:
  1. Click **+ Add Academic Year**.
  2. Enter **Year Name** (e.g., `Academic Year 2025-2026`).
  3. Pick **Start Date** (e.g., `01-Sep-2025`) and **End Date** (e.g., `30-Jun-2026`).
  4. Toggle **Current Year** to `ON` if this is the active school session.
  5. Click **Save**.

### 1.2 Grades & Sections
* **Navigation**: `Academic Management` > `Grade` & `Section`
* **Step-by-Step Instructions**:
  1. In **Grade Master**, click **+ Add Grade**. Specify Grade Name (e.g., `Grade 10`) and display sequence order.
  2. In **Section Master**, click **+ Add Section**. Create required section divisions (e.g., `A`, `B`, `C`).
  3. In **Grade Section Mapping**, link grades to their sections and set maximum student capacity per class.

### 1.3 Subjects & Curricular Mapping
* **Navigation**: `Academic Management` > `Subjects`
* **Step-by-Step Instructions**:
  1. Click **+ Add Subject**.
  2. Enter **Subject Code** (e.g., `ENG101`), **Subject Name** (e.g., `English Language & Literature`), and **Credit Hours**.
  3. Mark as *Core*, *Elective*, or *Language Option*.
  4. Assign the applicable grading method (Marks-based or Rubrics-based).

### 1.4 Class Teacher Allocation
* **Navigation**: `Academic Management` > `Class Teacher Allocation`
* **Step-by-Step Instructions**:
  1. Click **Allocate Class Teacher**.
  2. Select **Academic Year**, **Grade**, and **Section**.
  3. Select the faculty member from the **Teacher** dropdown.
  4. Click **Save**. The allocated teacher immediately receives homeroom security rights for student attendance, report cards, and parent communications.
  5. Use the **Filter Drawer** to view assignments by grade or teacher, and click **Export** to produce the class teacher directory.

---

## Module 2: Admissions & Student Lifecycle Management
> **Primary Users**: Admissions Officers, Registrars, Front Office

### 2.1 Student Registration Desk
* **Navigation**: `Admission Management` > `Admission Register`
* **Step-by-Step Instructions**:
  1. Click **+ New Admission**.
  2. **Student Profile**: Enter Legal Full Name, Date of Birth, Gender, Blood Group, Nationality, and National Identity Number (Emirates ID / Civil ID).
  3. **Parent / Guardian Details**: Enter Father's and Mother's name, email addresses, primary contact mobile, and emergency numbers.
  4. **Class Enrolment**: Select **Admission Grade** and allocate an active **Section**.
  5. **Supporting Documents**: Upload digital copies of Birth Certificate, Passport, Immunization Record, and Previous School Transfer Certificate.
  6. Click **Submit**. The system auto-generates a unique **Student Registration Number (SRN)** and creates an active student profile.

### 2.2 Re-Registration Block / Unblock Desk
* **Navigation**: `Admission Management` > `Re-Registration Block / Unblock`
* **Purpose**: Controls eligibility for students to re-enroll into the next academic session. Used to place holds for overdue fee balances or documentation compliance.
* **Key Operating Controls**:
  - **KPI Metrics Bar**: Displays real-time counts for *Total Candidates*, *Eligible for Next Year*, *Blocked / On Hold*, and *Fee Arrears Defaulters*.
  - **Status Toggle Switch**: Flip the toggle on any student row between *Active (Eligible)* and *Blocked*.
  - **Filter Drawer**: Click **Filter** to filter candidate lists by Grade, Section, or Block Reason.
  - **Defaulter Auto-Hold**: Click **Auto-Hold Fee Defaulters** to automatically freeze all student accounts with overdue balances exceeding policy thresholds.
  - **Excel Export**: Click **Export** to download the complete re-registration status roster.

### 2.3 Transfer Certificates (TC) & Multi-Department Clearances
* **Navigation**: `Admission Management` > `Transfer Certificates & Clearances`
* **Purpose**: Automated end-to-end student exit and clearance workflow.
* **Clearance Flow**:
  1. **Initiate Request**: Click **+ New TC Request**. Search and select the student, specify Departure Date and Reason for Leaving.
  2. **Departmental Sign-offs**: Clearances route automatically to 5 departmental queues:
     - *Accounts*: Clears outstanding fee dues.
     - *Library*: Verifies return of all borrowed books.
     - *Sports & Labs*: Checks uniforms and laboratory equipment.
     - *Transport*: Verifies cancellation of bus service and stops.
     - *Clinic*: Releases immunization files and medical charts.
  3. **Final Release**: Once all 5 checkmarks turn green, the Registrar clicks **Issue Transfer Certificate**.
  4. The system produces the official QR-coded, ministry-compliant Transfer Certificate PDF.

---

## Module 3: Fee Management, Invoicing & Cashier Desk
> **Primary Users**: Cashiers, Accountants, Finance Managers

### 3.1 Fee Structures & Fee Terms
* **Navigation**: `Fee Management` > `Fee Structure` & `Fee Term`
* **Step-by-Step Instructions**:
  1. Create **Fee Categories**: Tuition, Laboratory Fee, Transport, Library, Extra-Curricular, Admission Fee.
  2. Define **Fee Terms**: Term 1 (Autumn), Term 2 (Spring), Term 3 (Summer), or Monthly Billing Cycles.
  3. In **Fee Structure Master**, build the matrix linking each Grade to its applicable fee components and payment due dates.

### 3.2 Invoicing & Fee Concessions
* **Navigation**: `Fee Management` > `Fee Invoices` & `Fee Concessions`
* **Step-by-Step Instructions**:
  1. **Bulk Invoicing**: Select Academic Year, Fee Term, and target Grades. Click **Generate Invoices**. Invoices are assigned to all enrolled students with breakdown itemization.
  2. **Concessions & Scholarships**: To apply sibling discounts, staff child allowances, or merit scholarships, open **Fee Concessions**, select the student, specify concession percentage or fixed amount, and attach authorization approval.

### 3.3 Fee Collection Desk (Point of Sale)
* **Navigation**: `Fee Management` > `Fee Collection`
* **Step-by-Step Instructions**:
  1. Search for the student by **SRN**, Student Name, or Parent Mobile.
  2. The screen displays the student's complete financial ledger: Total Billed, Total Paid, Overdue Balance, and Active Term Invoices.
  3. Select the invoice items to settle.
  4. Select **Payment Mode**: *Cash*, *Credit/Debit Card*, *Cheque / Post-Dated Cheque (PDC)*, or *Bank Transfer*.
  5. If paying by cheque, enter Cheque Number, Bank Name, and Cheque Maturity Date.
  6. Click **Process Payment**.
  7. The system issues an official printable **Fee Receipt Voucher** with institution branding and barcode.

### 3.4 Late Fines & Defaulter Follow-up
* **Navigation**: `Fee Management` > `Fee Late Fine` & `Fee Reminders`
* **Step-by-Step Instructions**:
  1. Configure fine rules (e.g., daily penalty or flat late fee after due date).
  2. Use **Fee Reminders** to send automated SMS/Email reminders to parents with overdue balances.
  3. To waive fines for valid reasons, open **Waive Fine Drawer**, enter the waiver amount, provide approval notes, and submit.

---

## Module 4: Learning Management System (LMS) & Curriculum
> **Primary Users**: Academic Heads, Subject Teachers, Curriculum Coordinators

### 4.1 Syllabus & Lesson Planning Tracker
* **Navigation**: `LMS` > `Curriculum Tracker`
* **Step-by-Step Instructions**:
  1. Select **Grade**, **Section**, and **Subject**.
  2. Review the chapter breakdown and planned instructional units.
  3. Teachers click **Update Progress** to mark topics as *Completed*, record actual teaching dates, and add pedagogical notes.
  4. Academic coordinators track curriculum pacing via the visual completion progress bar.

### 4.2 Digital Question Bank
* **Navigation**: `LMS` > `Question Bank`
* **Step-by-Step Instructions**:
  1. Click **+ Add Question**.
  2. Select Subject, Unit, and Topic.
  3. Select Question Type: *Multiple Choice (MCQ)*, *Short Answer*, *Descriptive Essay*, or *Fill in the Blanks*.
  4. Specify **Difficulty Level**: *Easy*, *Medium*, or *Hard*.
  5. Tag with **Bloom's Taxonomy Level** (*Remembering*, *Understanding*, *Applying*, *Analyzing*, *Evaluating*, *Creating*).
  6. Enter question text, grading criteria, and correct answer key.
  7. Questions are added to the institution's verified question repository for automated test paper generation.

### 4.3 Test Paper Generator
* **Navigation**: `LMS` > `Test Paper Generator`
* **Step-by-Step Instructions**:
  1. Click **Create Test Paper**.
  2. Define parameters: Total Marks, Duration (minutes), and difficulty distribution (e.g., 40% Easy, 40% Medium, 20% Hard).
  3. Select target units and chapters.
  4. Click **Generate Blueprint**. The system automatically selects questions conforming to your blueprint.
  5. Review, swap individual questions if desired, and click **Finalize & Export PDF**.

---

## Module 5: Examination Studio, Grading & Report Card Release
> **Primary Users**: Examination Officers, Class Teachers, Academic Directors

### 5.1 Examination Scheduling & Timetable
* **Navigation**: `Exam Management` > `Exam List`
* **Step-by-Step Instructions**:
  1. Click **+ Create Exam**.
  2. Enter Exam Title (e.g., `Term 1 Final Assessment 2025-2026`).
  3. Configure the assessment schedule: assign dates, start/end times, and room locations for each subject.
  4. Set Maximum Marks, Minimum Pass Marks, and Weightage percentage.

### 5.2 Marks Entry Desk
* **Navigation**: `Exam Management` > `Marks Entry`
* **Step-by-Step Instructions**:
  1. Select **Academic Year**, **Exam Series**, **Grade**, **Section**, and **Subject**.
  2. The class roster is loaded into the marks entry grid.
  3. Enter student scores. The system provides immediate validation warnings if an entered score exceeds maximum marks.
  4. Mark absent students using the *Absent (AB)* or *Medical Exemption (ML)* flag.
  5. Click **Save Draft** during entry, and click **Submit for Result Compilation** once completed.

### 5.3 Report Card Studio & Remarks
* **Navigation**: `Exam Management` > `Report Card Studio`
* **Step-by-Step Instructions**:
  1. Select the Report Card Template (CBSE, Ministry of Education, British Cambridge, IB, or American Standard).
  2. Class Teachers enter pastoral and behavioral comments (e.g., "Demonstrates exceptional critical thinking in mathematics").
  3. Principals review class distributions and authorize final sign-off.

### 5.4 Report Card Withholding & Portal Release Desk
* **Navigation**: `Exam Management` > `Report Card Block / Unblock`
* **Purpose**: Prevents students and parents with outstanding fee arrears or disciplinary holds from viewing or downloading report cards from their web/mobile portals.
* **Key Operating Controls**:
  - **KPI Cards Bar**: Displays *Total Results Compiled*, *Published to Portal*, *Withheld on Hold*, *Fee Defaulters*, and *Admin Overrides*.
  - **Portal Release Toggle Switch**: Toggle between *Published (Visible on Portal)* and *Withheld*.
  - **Filter Drawer**: Filter candidates by Academic Year, Exam Series, Grade, Section, or Release Status.
  - **Excel Export**: Export the report card publishing ledger based on active filters.
  - **Bulk Release**: Click **Bulk Release Cleared Cards** to instantly publish report cards for all students with settled financial accounts.
  - **Emergency Admin Override**: For special circumstances, an authorized administrator can override an active fee hold to release a single report card with mandatory audit remarks.

---

## Module 6: Campus Transport & Fleet Operations
> **Primary Users**: Transport Managers, Bus Coordinators

### 6.1 Bus Routes & Stops
* **Navigation**: `Transport Management` > `Routes`
* **Step-by-Step Instructions**:
  1. Click **+ Add Route**. Enter Route Code (e.g., `RT-04-North`) and Route Name.
  2. Define stops in pickup sequence with scheduled pickup and drop-off times.
  3. Assign route monthly/term fare pricing.

### 6.2 Vehicle & Driver Allocation
* **Navigation**: `Transport Management` > `Vehicles & Drivers`
* **Step-by-Step Instructions**:
  1. Register bus fleet: Registration Number, Capacity, Insurance Expiry, and RTA/DOT Permit Details.
  2. Assign licensed Driver and Bus Attendant (Nanny/Conductor).
  3. Assign students to designated stops. The system generates digital student bus manifests with emergency contact numbers.

---

## Module 7: Human Resources, Staff & Payroll Management
> **Primary Users**: HR Managers, Administrative Directors

### 7.1 Staff Directory & Onboarding
* **Navigation**: `HR Management` > `Staff Directory`
* **Step-by-Step Instructions**:
  1. Click **+ Add Staff**.
  2. Record Personal Details: Full Legal Name, Nationality, Civil/Emirates ID, Contact Information, and Educational Credentials.
  3. Record Employment Details: Department, Designation, Joining Date, Contract Type, and Basic Salary.
  4. Assign one or more of the **27 Tenant Operational Roles** (e.g., Teacher, Accountant, Admissions Officer, Clinic Nurse).
  5. Upload compliance documents: Employment Visa, Labor Contract, Teaching License, Police Clearance.

### 7.2 Staff Attendance & Leave Management
* **Navigation**: `HR Management` > `Staff Attendance` & `Leave Applications`
* **Step-by-Step Instructions**:
  1. Daily attendance synchronizes via biometric/RFID readers or manual supervisor entry.
  2. Staff submit leave requests via their employee portal (Annual, Sick, Maternity, Emergency).
  3. HR Managers review leave balances, check replacement teacher allocations, and click **Approve** or **Reject**.

---

## Module 8: Clinic & Student Health Management
> **Primary Users**: School Nurses, Medical Doctors, Health Officers

### 8.1 Electronic Health Records (EHR)
* **Navigation**: `Health & Clinic` > `Health Profiles`
* **Step-by-Step Instructions**:
  1. Search for any enrolled student to access their comprehensive medical file.
  2. Record chronic medical conditions, severe allergies (e.g., Peanuts, Penicillin), dietary restrictions, and emergency inhaler/EpiPen locations.
  3. Allergy flags automatically alert homeroom teachers and cafeteria staff.

### 8.2 Daily Clinic Visits & Vaccination Scheduler
* **Navigation**: `Health & Clinic` > `Daily Visits` & `Vaccination Scheduler`
* **Step-by-Step Instructions**:
  1. When a student visits the clinic, click **Log Clinic Visit**.
  2. Record Symptoms, Temperature, Blood Pressure, and Administered Treatment / Medication.
  3. Mark Disposition: *Returned to Class*, *Sent Home*, or *Referred to Hospital*.
  4. If sending home, an automated SMS alert is dispatched to parents.
  5. Track mandatory statutory vaccination campaigns using the **Vaccination Scheduler**.

---

## Module 9: School Finance & Accounting Hub
> **Primary Users**: Chief Financial Officers, Senior Accountants

### 9.1 General Ledger & Vouchers
* **Navigation**: `Finance` > `Vouchers` & `Account Books`
* **Step-by-Step Instructions**:
  1. Daily fee receipts automatically generate balanced Journal Vouchers (Debit: Cash/Bank, Credit: Tuition Fee Income).
  2. Create manual vouchers: Payment Vouchers (Vendor expenses), Receipt Vouchers, Contra Vouchers (Bank-to-Cash), and Journal Vouchers.
  3. Multi-currency and tax-compliant (VAT / GST) posting engine.

### 9.2 Cheque & PDC Vault
* **Navigation**: `Finance` > `PDC Vault`
* **Step-by-Step Instructions**:
  1. View all post-dated student fee cheques organized by maturity date.
  2. Mark cheques as *Deposited*, *Cleared*, or *Bounced / Returned*.
  3. Bounced cheques automatically reverse fee receipts, re-open student fee invoices, and flag the student on the **Re-Registration Hold** and **Report Card Withholding** desks.

---

## Module 10: Parent & Student Self-Service Portal
> **Primary Users**: Parents, Students

### 10.1 Web & Mobile Portal Capabilities
- **Daily Attendance**: Real-time notification of student presence, late arrival, or unexcused absence.
- **Academic Timetable**: Weekly schedule with subject periods, classroom numbers, and teacher names.
- **Fee Desk & Online Payments**:
  - Review active term invoices and fee breakdowns.
  - Pay instantly using credit card, debit card, or Apple Pay/Google Pay via integrated payment gateways.
  - Download official payment receipts.
- **Homework & Learning Vault**: Download digital lesson notes, submit assignments, and review teacher feedback.
- **Examinations & Report Cards**:
  - View upcoming exam schedules and subject syllabi.
  - Access published Report Cards with interactive performance analytics (subject averages, class rankings, and historical progress).
  - *Note*: If an account is placed on financial or administrative withhold, the portal displays a respectful alert prompting the parent to contact the accounts office to clear dues.

---

## 11. Quick Reference: Daily, Termly & Annual School Calendar Tasks

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│                   INSTITUTIONAL OPERATIONAL TIMELINE                             │
├──────────────────────────────────────────────────────────────────────────────────┤
│ DAILY OPERATIONS:                                                                │
│  • Record Student & Staff Attendance (Morning 08:00 AM)                         │
│  • Process Fee Collections & Issue Payment Receipts                             │
│  • Log Clinic Visits & Dispatch Parent Medical Alerts                            │
│  • Monitor Transport Bus Tracking & Route Dispatches                             │
├──────────────────────────────────────────────────────────────────────────────────┤
│ TERMLY OPERATIONS:                                                               │
│  • Generate & Issue Term Fee Invoices                                            │
│  • Track Curriculum Progress Tracker in LMS                                     │
│  • Conduct Exam Assessments & Enter Subject Marks                                │
│  • Audit Defaulters & Manage Report Card Withholding Desk                        │
│  • Publish Cleared Report Cards to Parent Portal                                 │
├──────────────────────────────────────────────────────────────────────────────────┤
│ ANNUAL / YEAR-END OPERATIONS:                                                    │
│  • Create & Activate New Academic Year Session                                   │
│  • Review Re-Registration Candidate Lists (Auto-Hold Defaulters)                 │
│  • Execute Academic Year Rollover (Promote Students to Next Grade)               │
│  • Allocate Homeroom Class Teachers for New Session                              │
│  • Finalize Staff Contracts, Leave Rollover & Audit Accounts                     │
└──────────────────────────────────────────────────────────────────────────────────┘
```

---

## 12. Support & Assistance
If you encounter system exceptions, need custom report formats, or require role privilege adjustments, contact your school's IT System Administrator or log a ticket via the **Help & Support** tab in the top navigation bar.
