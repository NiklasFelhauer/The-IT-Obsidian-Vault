# 🏁 Sprint 6 Summary (Calendar Weeks 8–10)

## 🛠️ Key Tasks

### UI Development & AG Grid Integration
- Collaborated on a **UI spike** to explore the integration of AG Grid into the canvas-based application.
- Successfully:
  - Implemented dynamic data rendering with AG Grid.
  - Enabled filtering, floating filters, tooltips, and dropdowns for symbol classification.
  - Separated AG Grid into base and extended components (e.g., CanvasPageGrid).
  - Created handlers for row selection events to enable interaction with the canvas.
  - Explored integration of Siemens IX components and compared with existing UI frameworks (Simpk vs. IX).

### Backend Interaction
- Began **mapping functionalities** between the AG Grid and backend APIs to enable interactive features like accept/reject.

### Bugfixing
- Resolved issue where **adding a new row reset the canvas zoom and scroll position**.
  - Solution: Maintained focus and zoom unless grid edit mode was triggered, which still caused issues needing further investigation.

## 🎯 Achievements

- ✅ Completed the **UI spike** with a working AG Grid integration.
- ✅ Enabled dynamic UI elements, significantly improving flexibility and maintainability.
- ✅ Supported teammates (Luke, Farheen, Pulkit) with their technical issues.
- ✅ Finished and documented code in local branches and Obsidian.
- ✅ Passed theory exam for driver’s license with a perfect score — major personal achievement.

## ⚠️ Challenges

- ⚙️ Difficulty aligning team on UI tech stack (Simpk vs. IX); requires further discussion with team leads.
- 🧩 Encountered **complex canvas interaction issues** when editing AG Grid rows — postponed deeper work until AG Grid integration stabilizes.
- 🧠 Sprint week included personal time off and reduced availability due to driver’s license lessons and health-related appointments.

## 📌 Next Steps

- Finalize AG Grid and Canvas integration logic (e.g., preserve zoom on interaction).
- Implement action buttons (accept/reject) and bind them to backend APIs.
- Clarify team decisions on UI framework and merge ongoing refactors (Paul’s changes).
- Plan next Sprint based on solid AG Grid foundation and UX concepts from Prajacta.

---

Prepared for Sprint Review by: [Your Name]
Sprint 6 | Weeks 8–10

