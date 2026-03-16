# Hero Network — Platform Workflow

> **Purpose:** Provides the SEO content machine with an accurate, step-by-step walkthrough of the Hero Network user experience — from sign-up through delivery. Reference this document to describe the actual product experience, use correct terminology, and ensure CTAs reference real UI elements.

---

## Key Terminology

| Term | Definition |
|------|-----------|
| **Host** | The primary user of the platform — the creator, agency owner, or content producer who manages clients and projects. |
| **Guest** | The person being recorded. Guests do not need a Hero Network account. |
| **Client** | Top-level organizational unit. Every project must belong to a Client. Clients persist across projects. |
| **Project** | A single recording/editing job within a Client. Contains recordings, uploaded assets, editing briefs, and deliverables. |
| **Smart Library** | Hero Network's client-level Digital Asset Management (DAM) system. Any media recorded or uploaded to a project is stored in the Client's Smart Library for reuse across projects. |
| **Guest Link** | A unique invitation (email or SMS) sent to a Guest to join a live recording session. No app install or account required. |

---

## Complete User Journey

### 1. Sign-Up & Onboarding

New Hosts go through a guided setup flow that covers:

1. Account creation (name, email, password)
2. Create their first Client
3. Upload brand assets (logos, colors, fonts) to the Client's Smart Library
4. Invite team members (if applicable)
5. Create their first Project

After onboarding, the Host lands on their dashboard with their first Client and Project ready to go.

### 2. Creating a Project

The Host creates a new Project under an existing Client. Each Project is the container for a single recording/editing job.

- Projects inherit access to the Client's Smart Library (logos, B-roll, brand assets)
- Hosts can upload additional project-specific assets (B-roll, reference materials, supplementary media)
- Both project-level uploads and Client-level assets are available to editors

### 3. Setting Up Guests

Guests are the people the Host will record with. Key details:

- Guests are created within the platform and **saved for reuse** across projects
- No Guest account or app install is required — recording happens in the Guest's mobile browser
- Hosts send invitations to Guests via **email or SMS**
- Scheduling and calendar invites are available for planned sessions

### 4. The Live Recording Session

Hero Network has a **built-in, high-fidelity video recorder** — not a Zoom integration or third-party tool.

**Host experience (desktop):**
- Starts or joins the recording session from the Project
- Sees the Guest's video feed in real-time — full video call experience
- Controls the recording (start, stop, pause)
- Can interact naturally with the Guest during recording

**Guest experience (mobile browser):**
- Receives an invitation link via email or SMS
- Opens the link in their mobile browser — no app download, no account creation
- Joins the live session and records using their phone's camera
- High-fidelity camera resolution captured directly from the mobile device

**Technical architecture:**
- Video is captured using packeted chunk uploads — footage is uploaded in real-time during the recording session
- Chunks are stitched together in AWS and delivered seamlessly to the Host's Project
- By the time the session ends, the footage is already uploaded — no manual upload step required

### 5. Post-Recording: Preparing for Editing

After the recording session, the footage auto-uploads to the Project. The Host then:

1. **Reviews the recording** in the Project
2. **Uploads additional assets** if needed (B-roll, supplementary footage, reference clips) — these also go to the Client's Smart Library for cross-project reuse
3. **Submits for editing** with a structured brief that includes:
   - Structured options (deliverable types, style preferences, target length, specific cuts requested)
   - Free-form editing notes (custom instructions, timestamps to highlight, creative direction)

The Host specifies exactly what deliverables they want — full episode, social clips, vertical shorts, or any custom combination.

### 6. Editing & Status Tracking

Once submitted, the Project enters the editing pipeline:

- **Status tracking:** The Host can monitor editing progress in the platform via status indicators
- **Turnaround:** Standard delivery is **3–5 business days**
- Editors have access to both project-level assets and the Client's Smart Library (brand assets, logos, previously uploaded B-roll)

### 7. Review & Revision Cycle

When editing is complete:

- **In-app delivery:** Finished edits appear directly in the Project
- **Email notification:** The Host receives an email alerting them that edits are ready for review
- **In-platform review:** The Host reviews the deliverables within Hero Network
- **Revision requests:** If changes are needed, the Host submits revision notes and the editor makes adjustments

### 8. Final Delivery

Once the Host approves the edit:

- Final deliverables are available for download from the Project
- All media (raw footage, B-roll, final edits) remains stored in the Client's Smart Library for future use across projects

---

## What Makes This Different

When writing about Hero Network's workflow, emphasize these differentiators:

- **Built-in high-fidelity recorder** — not a Zoom plugin or screen recorder. Purpose-built for professional remote video capture.
- **Zero friction for Guests** — link-only access via mobile browser. No downloads, no accounts, no technical setup.
- **Smart Library (Client DAM)** — assets persist across projects. Record once, reuse everywhere. Editors always have access to brand assets.
- **Real-time chunk uploads** — footage uploads during the recording session via packeted chunks stitched in AWS. No waiting for uploads after the session ends.
- **End-to-end platform** — recording, asset management, editing briefs, status tracking, review, and delivery all happen in one place.

---

## Content Guidelines

- Always use "Host" (not "user" or "creator") when referring to the primary platform user
- Always use "Guest" (not "interviewee" or "participant") for the person being recorded
- Always use "Client" as the top-level organizational unit — never imply projects exist independently
- Reference "Smart Library" when discussing asset management and cross-project reuse
- Never describe the recording as a "Zoom call" or suggest third-party recording tools are needed
- Never say "upload your video" — the upload is automatic during recording
- CTAs should reference real actions: "Create your first project," "Send a Guest link," "Submit for editing"
