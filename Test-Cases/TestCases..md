# Test Cases – RemoteAxle

## TC-001: Verify homepage loads successfully

**Module:** Homepage

**Description:** Test if the homepage loads smoothly when accessed.

**Steps to Reproduce:**

1. Go to https://remoteaxle.com
2. Observe homepage loading

**Expected Result:**

Homepage should load without errors.

---

## TC-002: Verify course listing page loads

**Module:** Courses Module

**Description:** To check if the course listing page displays available courses.

**Steps to Reproduce:**

1. Go to https://remoteaxle.com
2. Click "Browse Our Courses" or "Explore Courses"

**Expected Result:**

Course listing page should display all available courses.

---

## TC-003: Verify course filters work correctly

**Module:** Courses Module

**Description:** To verify that filters display courses belonging to the selected category.

**Steps to Reproduce:**

1. Go to https://remoteaxle.com
2. Click "Explore Courses"
3. Select a category filter
4. Observe displayed courses

**Expected Result:**

Only courses related to the selected category should be displayed.

---

## TC-004: Verify courses added to cart appear in cart

**Module:** Cart Module

**Description:** Verify that courses added to cart are listed in the cart with their fee.

**Steps to Reproduce:**

1. Go to homepage
2. Click "Explore Courses"
3. Select any course
4. Click "Add to Cart"
5. Click cart icon

**Expected Result:**

The selected course should appear in the cart with the correct price.

---

## TC-005: Verify payment methods work correctly

**Module:** Payment Module

**Precondition:** User must be logged in and have items in cart.

**Steps to Reproduce:**

1. Go to homepage
2. Click "Cart"
3. Select payment method
4. Click "Enroll Now"

**Expected Result:**

User should be redirected to the selected payment gateway.

---

## TC-006: Verify login with valid credentials

**Module:** Login Module

**Precondition:** User must be registered.

**Test Data:**

Email: test@test.com  
Password: 12aa34bb56

**Steps to Reproduce:**

1. Go to homepage
2. Click "Login"
3. Enter valid credentials
4. Click "Log in"

**Expected Result:**

User should log in successfully.

---
### TC-007: Add Course to Cart

**Module:** Course Page  
**Priority:** High  
**Type:** Functional

**Preconditions**
- User is on the course listing page

**Test Steps**
1. Navigate to https://remoteaxle.com
2. Click "Explore Courses"
3. Select any course
4. Click "Add to Cart"

**Expected Result**
- The course should be added to the cart
- Cart icon should show updated item count
- User should see confirmation feedback
---
### TC-008: Cart Persistence Across Pages

**Module:** Cart  
**Priority:** High  
**Type:** Functional

**Preconditions**
- A course is already added to cart

**Test Steps**
1. Add a course to the cart
2. Navigate to another page (Home / Courses)
3. Return to the cart page

**Expected Result**
- Previously added course should still be visible in cart
- Cart count should remain correct
---
### TC-009: Remove Course from Cart

**Module:** Cart  
**Priority:** Medium  
**Type:** Functional

**Preconditions**
- At least one course is present in the cart

**Test Steps**
1. Navigate to the cart page
2. Click the remove/delete option for a course

**Expected Result**
- Course should be removed from cart
- Cart count should update accordingly
- Empty cart message should appear if no items remain
---
## TC-010: Login With Invalid Password

**Module:** Login

**Description:** Verify that login fails when an incorrect password is entered.

**Precondition**
User must already be registered.

**Test Data**
Email: test@test.com  
Password: 12aa34bb33

**Steps to Reproduce**
1. Go to homepage
2. Click **Login**
3. Enter valid email and incorrect password
4. Click **Log In**

**Expected Result**
Error message **"Incorrect Password"** should be displayed

---
## TC-011: Signup With Valid Email

**Module:** Signup

**Description:** Verify that a new user can sign up using valid details.

**Steps to Reproduce**
1. Go to homepage
2. Click **Sign Up**
3. Enter valid credentials
4. Click **Create Account**

**Test Data**
First Name: XYZ  
Last Name: ABC  
Email: test@test.com  
Password: 12aa34bb56

**Expected Result**
Account should be created successfully with confirmation message.

---
## TC-012: Password Must Be At Least 8 Characters

**Module:** Signup

**Description:** Verify password validation during signup.

**Steps to Reproduce**
1. Go to homepage
2. Click **Sign Up**
3. Enter required details
4. Enter passwords with different lengths

**Test Data**
Passwords Tested:
- 12aa33bb
- 112cccc
- 112233445

**Expected Result**
Passwords with fewer than 8 characters should show error  
**"Password must be at least 8 letters."**
