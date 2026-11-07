E-HADIR UiTM
Student Event & Workshop Ticketing System
CSC584 - Enterprise Programming
HTML STORYBOARD / PROTOTYPE
============================================

1. PROJECT OVERVIEW
E-Hadir UiTM is a proposed university event and workshop ticketing system for three roles: Student, Committee, and Administrator. This submission is an HTML/CSS/JavaScript storyboard and demonstrates the intended interface and navigation. It is NOT the final Java MVC web application.

2. HOW TO OPEN THE STORYBOARD
- Extract the complete ZIP archive before opening the project.
- Open storyboard.html in a modern web browser (Google Chrome recommended).
- Use the module links or the Open HTML Page links to inspect each page.
- Open index.html to try the prototype Login page and demo navigation links for Student, Committee, and Admin.
- Keep the same browser tab when testing workflows that use sessionStorage.
- A local web server may be needed if browser security settings restrict storage on file:// pages.

3. MODULES AND HTML FILES
Common:
  index.html                  - Login page and demo role navigation
  register.html               - Student account registration validation

Student:
  student-dashboard.html      - Student dashboard
  events.html                 - Browse university events
  event-details.html          - Event details
  event-registration.html     - Demo event registration confirmation
  digital-ticket.html         - Demo digital ticket

Committee:
  committee-dashboard.html    - Committee dashboard
  manage-events.html          - Event listing and view links
  create-event.html           - Create event validation and preview
  edit-event.html             - Edit workshop data in sessionStorage
  attendance.html             - Demo attendance tracking and summary

Administrator:
  admin-dashboard.html        - Cancelled-event deletion demonstration

4. SYSTEM DOCUMENTATION
- documentation/system-navigation-flowchart.png
- documentation/system-navigation-flowchart.mmd
- documentation/ehadir-final-erd.png
- documentation/ehadir-final-erd.mmd

The ERD documents five Apache Derby entities:
USERS, CATEGORIES, EVENTS, REGISTRATIONS, and ATTENDANCE.

5. SCREENSHOT GALLERY
screenshots/ contains 13 PNG files (01-login.png through
13-admin-dashboard.png). These screenshots are displayed in
storyboard.html and correspond to the 13 HTML prototype pages.

6. DEMONSTRATION NOTES AND LIMITATIONS
- Login links are for storyboard navigation only; no real user authentication or role-based access control is enforced.
- Registration validation is a browser-side demonstration.
- Create Event validates inputs and displays a preview; it does not INSERT into Apache Derby.
- Edit Event uses sessionStorage for temporary browser-tab data.
- Event Registration and Digital Ticket use sessionStorage as a demo flow; the ticket is not valid for event entry.
- Attendance selections and summaries use sessionStorage; they are not saved to Apache Derby.
- Delete Event removes the HTML table row after confirmation; no database record is deleted, and refresh restores the sample row.
- The HTML pages use sample data; some default content may remain static. Data in sessionStorage is temporary and is not shared between browsers or devices.
- The database schema/ERD was developed separately in Apache Derby. This ZIP does not include an active database server or a working Java MVC backend.

7. FOLDER REQUIREMENTS
Keep storyboard.html, all 13 HTML pages, and style.css in the same root folder. Preserve images/, screenshots/, and documentation/ with their original file names and relative paths. Do not move or rename files without updating their HTML references.

8. NEXT DEVELOPMENT PHASE
The final application is planned to use JavaBeans, JSP, Servlets, JDBC, and Apache Derby for real authentication, event operations, registration, digital tickets, and attendance management.

END OF README
