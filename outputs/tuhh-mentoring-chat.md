# TUHH Mentoring Platform — Chat Record

## Referenced earlier conversation: “Guide Matching Tool”

**User:** Please provide a list of the top 3 mentors for each mentee. The student can contact the mentors based on this list. The quickest student occupies his preferred mentor.

**Outcome:** The platform should give each mentee a ranked Top 3 list. The mentee initiates contact, and the mentor accepts or declines. The database records the request timestamp so the first confirmed contact receives the mentor’s available capacity. Participants do not see scores or matching explanations; Career Center administrators do.

**User:** Do you need additional information for building a first frontend for an app that user can use with their desktop?

**Outcome:** A browser-based desktop prototype was recommended, with demo logins for Mentee, Mentor, and Career Center/Admin. Proposed core views were login, profiles/questionnaires, Top 3 recommendations, request flow, and an admin dashboard.

**User:** bitte eine web app in einem desktop browser, simpler demo account, TUHH branded

**Outcome:** Confirmed: desktop-browser web app, simple demo account, and TUHH-branded design.

---

## Current project conversation

**User:** Build the first frontend prototype as a desktop-browser web app for the TUHH mentoring matching platform. Use a simple demo-account login (no real authentication). Make it TUHH-branded with a clean professional university style. Use the existing requirements and fictional prototype data from the conversation: 5 mentees and 5 mentors, 3 roles (Mentee, Mentor, Career Center/Admin), 6-question profiles, ranked Top 3 recommendations with no scores/reasons visible to participants, contact/accept/decline workflow, temporary deactivation/profile status, mentor capacity, and an admin dashboard with matching details. Focus on a polished clickable frontend prototype rather than backend integration. Use sensible mock state/data so the main flows can be demonstrated in the browser.

**Assistant:** Created a self-contained TUHH-branded clickable prototype. It has Mentee, Mentor, and Career Center demo logins; participant profiles; mentee Top 3 recommendations; availability and capacity controls; request and decision flows; and an admin-only matching view with detail and score placeholders. It includes five fictional mentees and five fictional mentors in the administration list.

**Deliverable:** [TUHH mentoring prototype](tuhh-mentoring-prototype.html)

**User:** Can you insert a button in order to switch between German and Englisch; before sending a contact request to the mentor the mentee should be able to see the mentors profile; The student should see that he sent out a message to the mentor; how does the mentor see the request?

**Assistant:** Updated the prototype with:

- An English/German switch in the application header.
- A **View profile** action for mentees, which shows the mentor’s experience, support areas, languages, and availability before the contact action.
- A visible **Request sent today** status for the mentee, plus a detailed mentoring-status page.
- A mentor-side **Connection requests** view. In the demo, sign out, select **Mentor · Michael Weber**, then open **Connection requests**. Michael sees Aisha’s study programme, interests, goals, languages, and availability, and can accept or decline.

**Updated deliverable:** [TUHH mentoring prototype](tuhh-mentoring-prototype.html)

---

## Prototype navigation guide

1. Start as **Mentee · Aisha Rahman**.
2. Open **My recommendations** and choose **View profile** for Michael Weber.
3. Choose **Send contact request**.
4. Review **My mentoring status** to see the sent request.
5. Sign out and choose **Mentor · Michael Weber**.
6. Open **Connection requests**, then accept or decline the request.
7. Sign out and choose **Career Center · Admin** to view matching information and programme activity.
