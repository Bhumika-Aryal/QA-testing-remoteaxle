# RemoteAxle Bug Reports

This document contains bugs identified during exploratory testing of https://remoteaxle.com

---
## BUG-001: Social Media Icons Redirect to Same URL

Module: Footer  
Severity: Low  
Priority: High  
Environment: Chrome, Windows 11

Description  
Social media icons in the footer (Facebook, Instagram, LinkedIn) all redirect to the same incorrect URL.

Steps to Reproduce
1. Go to https://remoteaxle.com
2. Scroll to the footer section
3. Click on each social media icon

Expected Result  
Each icon should navigate to its respective social media page.

Actual Result  
All icons redirect to the same URL which returns a **403 Forbidden** response.

---

## BUG-002: Privacy Policy Link Does Not Display Policy Content

Module: Footer  
Severity: Medium  
Priority: High  
Environment: Chrome, Windows 11

Description  
The Privacy Policy link does not display any privacy policy content.

Steps to Reproduce
1. Go to https://remoteaxle.com
2. Scroll to the footer
3. Click **Privacy Policy**

Expected Result  
User should be redirected to a page displaying the privacy policy.

Actual Result  
Page displays only footer content and no privacy policy information.


---
## BUG-003: Course Fee Not Displayed on Course Cards

Module: Courses  
Severity: Low  
Priority: High  
Environment: Chrome, Windows 11

Description  
Course cards do not display course fees. Users must open the course to see the price.

Steps to Reproduce
1. Go to https://remoteaxle.com
2. Click **Explore Courses**
3. Observe the course cards

Expected Result  
Course cards should display course fee.

Actual Result  
Course fee is not visible on the cards.


---
## BUG-004: Course Cards Overlap Each Other

Module: Courses UI  
Severity: Low  
Priority: Medium  
Environment: Chrome, Windows 11

Description  
Course cards appear too close to each other, making them visually difficult to distinguish.

Steps to Reproduce
1. Go to homepage
2. Click **Browse Our Courses**
3. Observe the course cards layout

Expected Result  
Cards should have proper spacing and margins.

Actual Result  
Cards appear visually overlapping.


---
## BUG-005: Default Instructor Bio Displayed When Bio Is Empty

Module: Course Page  
Severity: Low  
Priority: High  
Environment: Chrome, Windows 11

Description  
If instructor bio is empty, the system displays default placeholder text.

Steps to Reproduce
1. Go to https://remoteaxle.com
2. Click **Browse Courses**
3. Open any course
4. Scroll to **Instructor Section**

Expected Result  
If bio is empty, the section should remain blank or hidden.

Actual Result  
Default text **"This is bio about the user"** is displayed.

---
## BUG-006: Explore Workshops Button Not Working

Module: Workshops  
Severity: Low  
Priority: Medium  
Environment: Chrome, Windows 11

Description  
The **Explore Workshops** button does not navigate to any content.

Steps to Reproduce
1. Go to https://remoteaxle.com
2. Click **Workshops**
3. Click **Explore Workshops**

Expected Result  
User should be redirected to workshop content.

Actual Result  
Button does not perform any action.

---
## BUG-007: Email Field in Enquiry Form Not Properly Validated

Module: Enquiry Form  
Severity: Medium  
Priority: High  
Environment: Chrome, Windows 11

Description  
The enquiry form accepts invalid email addresses.

Steps to Reproduce
1. Go to https://remoteaxle.com
2. Open any course
3. Click **Send Enquiry**
4. Enter invalid email (example: aa@)

Expected Result  
System should display an email validation error.

Actual Result  
Invalid email is accepted and enquiry is submitted.

---
## BUG-008: Cart Total Amount Not Updating

Module: Cart  
Severity: Medium  
Priority: High  
Environment: Chrome, Windows 11

Description  
Cart displays added courses but does not show course fee or update the total amount.

Steps to Reproduce
1. Login to the site
2. Add any course to cart
3. Click on cart icon

Expected Result  
Cart should display course fee and updated total amount.

Actual Result  
Cart shows **Rs.0** and does not display course fee.

---

## BUG-009: Server Frequently Returns 522 Error

Module: Server / Performance  
Severity: High  
Priority: High  
Environment: Chrome, Windows 11

Description  
Website frequently fails to load course content and returns a **522 server error**.

Steps to Reproduce
1. Go to https://remoteaxle.com
2. Click **Browse Our Courses**
3. Observe response

Expected Result  
Server should respond with **200 OK** and load content normally.

Actual Result  
Server returns **522 error** and content fails to load.

---
## BUG-010: Notification Does Not Navigate to Related Section

Module: Notifications  
Severity: Medium  
Priority: Medium  
Environment: Chrome Browser

Description  
Clicking on notifications does not redirect the user to the related section or content.

Steps to Reproduce
1. Log in to https://remoteaxle.com
2. Click on the **Notifications** icon
3. Select any notification
4. Observe system behaviour

Expected Result  
User should be redirected to the related page or section referenced in the notification.

Actual Result  
Clicking the notification does not navigate anywhere.



