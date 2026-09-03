# Privacy Policy for JuPuente

**Last Updated:** September 3, 2026

This Privacy Policy explains how **JuPuente** ("we", "our", or "the extension"), an internal Chrome extension developed for Guzman Law Firm, handles user information, authentication credentials, and bankruptcy case workflow data.

---

## 1. Overview & Scope

JuPuente is an enterprise workflow assistant designed to streamline bankruptcy case management, claims reconciliation, and docket analysis within Jubilee Pro, Chapter 13 Trustee portals, and Southern District of Texas (SDTX) bankruptcy systems for authorized firm personnel.

JuPuente is committed to protecting user privacy, attorney-client privilege, and confidential bankruptcy case information. **We do not sell, rent, monetize, or trade any user or client data.**

---

## 2. Information We Collect

### A. User Authentication & Identity
- **Google Account Email Address:** When users sign in via Google OAuth2 (`chrome.identity`), we receive their Google email address solely to verify whether they are an authorized staff member or administrator on the firm's approved staff roster.
- We do not access passwords, contacts, Google Drive files, or personal emails.

### B. Application Preferences & State
- **Local Settings:** The extension stores local user interface preferences (such as collapsed sections, quick phrases, and active tab preferences) locally on your device via `chrome.storage.local`.
- **User Roles:** Authorized staff roles (Admin, Staff, Paralegal) assigned by the firm are stored securely to regulate access to administrative configuration panels.

### C. Case & Docket Workflow Data
- **Case Data Processing:** When authorized users view bankruptcy cases in Jubilee Pro or Trustee portals (e.g., 13Network, NDC), JuPuente parses docket numbers, hearing dates, claims, and case metadata strictly within the local browser session to render workflow badges, calculate deadlines, and facilitate document drafting.
- **Air-Gapped Processing:** Sensitive client document comparisons (such as PDF redlining) occur entirely in local browser memory without transmission to external servers.

---

## 3. How We Use Information

Information accessed by JuPuente is used exclusively for:
1. **Authentication & Access Control:** Ensuring only verified Guzman Law Firm staff access firm-specific automation tools and admin controls.
2. **Workflow Automation:** Populating hearing notices, matching trustee claims data, and surfacing case deadlines.
3. **Firm Configuration Sync:** Synchronizing firm-approved phrase dictionaries, note marks, and court hearing dates across authorized firm devices via Google Cloud Firestore.

---

## 4. Third-Party Services & Data Sharing

JuPuente connects only to designated services necessary for bankruptcy legal practice:
- **Google Identity Services / OAuth2:** For staff authentication.
- **Google Cloud Firestore (`firestore.googleapis.com`):** For synchronizing firm-level settings, staff roles, and court calendar dates. Governed by Google Cloud's Enterprise Security and Privacy Standards.
- **National Data Center (`api.ndc.org`):** For retrieving Chapter 13 case and plan payment status using firm-authorized credentials.
- **Chapter 13 Trustee Portals (`13network.com`, `ch13hou.com`, `ch13cctx.com`):** Direct navigation and data extraction for trustee recommendation dockets.

**We do not share any user data with third-party advertisers, data brokers, or external commercial entities.**

---

## 5. Permissions Justification

JuPuente requests the following Chrome extension permissions strictly for its operational features:
- `identity`: Authenticates firm staff via Google OAuth2 to enforce role-based access.
- `storage`: Persists local user preferences and cached firm configuration offline.
- `scripting` & `tabs`: Injects workflow UI components and status badges onto authorized Jubilee Pro and Trustee web pages.
- `declarativeNetRequest`: Handles secure header routing for internal API proxies.
- `alarms`: Schedules periodic background synchronization of court dockets and calendar events.
- `notifications`: Alerts staff of critical case deadlines or successful data synchronization.

---

## 6. Data Retention and Deletion

- **Local Storage:** Users can clear all local extension data at any time through Chrome Extension Settings (`chrome://extensions`) or by removing the extension.
- **Account Disassociation:** When a staff member departs or is removed from the firm's authorized staff roster in the Admin Portal, their access is revoked immediately.

---

## 7. Security

JuPuente enforces strict security practices:
- All external communications occur over encrypted TLS/HTTPS connections.
- No remotely hosted executable code is loaded (strict Manifest V3 compliance).
- All document diffing and legal redlining operate in local browser memory to preserve attorney-client confidentiality.

---

## 8. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect enhancements in workflow capabilities or regulatory requirements. The "Last Updated" date at the top of this document will always reflect the current revision.

---

## 9. Contact Us

If you have questions, concerns, or requests regarding this Privacy Policy, please contact:

**Guzman Law Firm / JuPuente Development Team**  
Email: [support@guzmanlawfirm.com](mailto:support@guzmanlawfirm.com)  
Website: [https://github.com/mayurpatel77/ProjectJP](https://github.com/mayurpatel77/ProjectJP)
