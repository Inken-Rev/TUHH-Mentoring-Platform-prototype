# TUHH Mentoring Platform Prototype

A TUHH-branded, desktop-browser frontend prototype for a mentoring matching programme. It is a self-contained HTML demonstration with no backend, authentication service, database, or real email delivery.

## Start the prototype

Open [`tuhh-mentoring-prototype.html`](tuhh-mentoring-prototype.html) in a desktop browser.

Use one of the simple demo accounts on the login screen:

- **Mentee:** Aisha Rahman, MSc Mechanical Engineering
- **Mentor:** Michael Weber, Engineering Manager in automotive
- **Career Center:** Programme administration

## Core workflow

1. The mentee completes or updates a profile.
2. The platform shows a ranked Top 3 list of available mentors. Scores and matching reasons are not shown to participants.
3. The mentee opens a mentor profile, writes an optional request message, and sends a contact request.
4. The mentor receives the request in **Connection requests**, sees the profile summary and the mentee’s note, writes an optional reply, and accepts or declines.
5. The mentee sees the decision and reply in **My mentoring status**.
6. The Career Center can review detailed matching information and programme activity.

The first confirmed connection wins. A mentor’s capacity is reserved after acceptance.

## Included functionality

### Mentee

- Ranked Top 3 mentor recommendations
- Mentor-profile preview before a contact request
- Optional message included with a mentoring request
- Request-sent and mentoring-status views
- Mentor response displayed after acceptance or decline
- Temporary profile deactivation / reactivation
- Profile inputs for study details, interests, mentoring goals, language, availability, email address, and LinkedIn profile

### Mentor

- Availability pause / resume control
- Mentor capacity indication
- Incoming connection request with the mentee’s profile summary
- Mentee request message
- Optional reply message before accepting or declining
- Profile inputs for professional background, availability, capacity, email address, and LinkedIn profile

### Career Center / Admin

- Programme overview with participant and request indicators
- Matching overview with admin-only profile alignment and match score details
- Participant list for 5 mentees and 5 mentors
- Programme settings explanation for Top 3 recommendations and first-confirmed-contact allocation

### Notifications

The prototype models notification emails without sending real mail:

- A mentor sees an **Email notification sent** preview after a mentoring request.
- A mentee sees an **Email notification sent** preview after the mentor answers.
- Each preview includes a link that opens the relevant in-app page.

Real email delivery requires a backend, a mail provider, user authentication, and secure, production URLs.

## Language

Use the **DE / EN** control in the application header to switch the UI between German and English.

## Technical notes

- Deliverable: `tuhh-mentoring-prototype.html`
- Technology: standalone HTML, CSS, and JavaScript
- State: temporary browser-memory demo state; page reload resets interactive changes
- Data: fictional demonstration participants only
- Authentication: demo-account selection only

## Suggested next steps

1. Move the prototype to a component-based web app such as React, Next.js, or Vue.
2. Add real authentication through the TUHH identity provider.
3. Create a database for profiles, requests, capacity, timestamps, and matching results.
4. Implement the matching service and availability checks on the server.
5. Connect an approved transactional-email service and use authenticated deep links.
6. Add privacy, consent, accessibility, and GDPR review before any production use.
