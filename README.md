# Greens-Landscaping
QA Testing Portfolio: Functional, UI, and API testing for the Greens Landscaping web application.

Project Overview
This repository contains the complete QA documentation for the Greens Landscaping web application, a front-end project built with HTML, CSS, Bootstrap, and JavaScript. Testing covered five main pages: Home, Services, Equipment, About, and Quote.

Testing Scope & Tools Used
Manual Testing: 30+ test cases executed covering UI layout, navigation routing, form validation, and responsive design.

Bug Tracking: Jira (Kanban board used for logging and resolving 12 defects).

API Testing: Postman (Verified HTTP 200 server health for GET requests and tested a mock POST endpoint for Quote submissions).

Test Management: Excel (Used to build the master test matrix and track pass/fail states).

Key Defects Identified & Resolved:
Mobile Navigation: The Bootstrap JavaScript CDN link was broken on the Services page, causing the mobile hamburger menu to fail completely.

Broken Routing: The "Contact Us" button on the Quote page pointed to a missing file (404 error). Updated the href to correctly route to about.html.

Image Cropping: Absolute positioning and object-fit rules were cutting off the tops of the mower images on the Equipment page. Fixed by updating CSS and expanding the container width.

Footer Layout: The footer floated in the middle of the screen on pages with minimal text. Fixed by applying a CSS Flexbox layout (min-height: 100vh) to keep it pinned to the bottom.

Local Server API Quirk: Documented a known "Parse Error" in Postman caused by how Live Server handles headers during GET requests (no impact on actual data).

Portfolio Artifacts:
Greens_Landscaping_Test_Matrix.xlsx: The master test case sheet containing preconditions, steps, expected/actual results, and Jira cross-references.

Screenshots: See the /screenshots folder for views of the Jira board, detailed bug reports, and Postman API checks.
