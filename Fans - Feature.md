# Module: On Boarding

## Page: On Boarding

### Task: Create On Boarding Page UI

**User Story:**  
As a new user,  
I want to see an attractive onboarding screen with Songcry branding  
so that I can understand what the app is about and feel confident to proceed.

**Acceptance Criteria:**
- AC 1: Page displays Songcry logo prominently
- AC 2: App branding elements are visible
- AC 3: Sign up button is clearly displayed
- AC 4: Google, Facebook, and Apple sign up buttons are available
- AC 5: Login link is accessible

---

## Page: Set Password

### Task: Create Set Password Page UI

**User Story:**  
GIVEN user completes Set Username Page,  
As a new user,  
I want to see a password setup page  
so that I can create a secure password for my account.

**Acceptance Criteria:**
- AC 1: Page displays "Password" title
- AC 2: Password input field is prominently displayed with placeholder text
- AC 3: Password requirements text is shown below input field
- AC 4: Eye icon for show/hide password functionality is available
- AC 5: Next button is displayed at the bottom
- AC 6: Navigation back to previous page is available

---

### Task: Handle Password Input Validation

**User Story:**  
As a new user on Set Password Page,  
I want to see real-time validation of my password  
so that I know if my password meets security requirements.

**Acceptance Criteria:**
- AC 1: Password must be at least 8 characters long
- AC 2: Password must contain at least one uppercase letter
- AC 3: Password must contain at least one lowercase letter
- AC 4: Password must contain at least one number
- AC 5: Password must contain at least one symbol
- AC 6: Real-time feedback shows validation status
- AC 7: Requirements text updates to show which criteria are met

---

### Task: Handle Password Visibility Toggle

**User Story:**  
As a new user on Set Password Page,  
I want to toggle password visibility  
so that I can verify I've typed my password correctly.

**Acceptance Criteria:**
- AC 1: Eye icon is visible next to password input field
- AC 2: Clicking eye icon toggles between show/hide password
- AC 3: Icon changes appearance to indicate current state
- AC 4: Password field type changes between password and text

---

### Task: Handle Password Error States

**User Story:**  
As a new user on Set Password Page,  
I want to see clear error indicators when my password is invalid  
so that I can understand what needs to be corrected.

**Acceptance Criteria:**
- AC 1: Input field shows red border when password is invalid
- AC 2: Error messages are displayed below the input field
- AC 3: Specific error messages for each validation failure
- AC 4: Error states clear when password becomes valid

---

### Task: Handle Next Button Click from Set Password Page

**User Story:**  
As a new user on Set Password Page,  
I want to click the Next button with a valid password  
so that I can proceed to Set Account page.

**Acceptance Criteria:**
- AC 1: Next button is only enabled when password meets all requirements
- AC 2: Button click saves password securely
- AC 3: Button click navigates to Set Account page
- AC 4: Loading state is shown during password processing

---

### Task: Handle Back Navigation from Set Password Page

**User Story:**  
GIVEN user is on Set Password Page,  
As a new user,  
I want to click the back button  
so that I can return to the Set Username Page.

**Acceptance Criteria:**
- AC 1: Back button is visible and accessible
- AC 2: Back button click navigates to Set Username Page
- AC 3: Previous password input state is cleared for security
- AC 4: Navigation maintains user's previous input context

---

### Task: Handle Sign Up Button Click

**User Story:**  
As a new user,  
I want to click the sign up button  
so that I can proceed to choose my role in the app.

**Acceptance Criteria:**
- AC 1: Button click navigates user to choose role page

---

**Title:**  
Handle Google Sign Up Button

**User Story:**  
As a new user,  
I want to sign up using my Google account  
so that I can quickly create an account without manual registration.

**Acceptance Criteria:**
- AC 1: Button click redirects to Google OAuth flow
- AC 2: If authentication successful, navigate to set username page
- AC 3: If authentication fails, return to on boarding page

---

### Task: Handle Facebook Sign Up Button

**User Story:**  
As a new user,  
I want to sign up using my Facebook account  
so that I can quickly create an account using my existing social media profile.

**Acceptance Criteria:**
- AC 1: Button click redirects to Facebook OAuth flow
- AC 2: If authentication successful, navigate to set username page
- AC 3: If authentication fails, return to on boarding page

---

### Task: Handle Apple ID Sign Up Button

**User Story:**  
As a new user,  
I want to sign up using my Apple ID  
so that I can securely create an account with Apple's privacy features.

**Acceptance Criteria:**
- AC 1: Button click redirects to Apple ID flow
- AC 2: If authentication successful, navigate to set username page
- AC 3: If authentication fails, return to on boarding page

---

### Task: Handle Login Link Click

**User Story:**  
As an existing user,  
I want to click the login link  
so that I can access my existing account.

**Acceptance Criteria:**
- AC 1: Link click navigates user to existing user login page

---

## Page: Choose Role

**Title:**  
Create Choose Role Page UI

**User Story:**  
GIVEN user clicks Sign Up button on the On Boarding Page,  
As a new user,  
I want to see a role selection page  
so that I can choose whether I'm joining as a Fan or an Artist.

**Acceptance Criteria:**
- AC 1: Page displays clear role selection options
- AC 2: Fan button is prominently displayed
- AC 3: Artist button is prominently displayed
- AC 4: Page shows relevant descriptions for each role
- AC 5: Navigation back to previous page is available

---

### Task: Handle Fan Role Selection

**User Story:**  
As a new user,  
I want to select the Fan role  
so that I can proceed to confirm my choice and access fan-specific features.

**Acceptance Criteria:**
- AC 1: Fan button click navigates to Fan Role Confirmation page

---

### Task: Handle Artist Role Selection

**User Story:**  
As a new user,  
I want to select the Artist role  
so that I can proceed to confirm my choice and access artist-specific features.

**Acceptance Criteria:**
- AC 1: Artist button click navigates to Artist Confirmation page

---

# Module: Sign Up

## Page: Fan Role Confirmation

### Task: Create Fan Role Confirmation Page UI

**User Story:**  
GIVEN user selects Fan role on Choose Role Page,  
As a new user,  
I want to see a confirmation page for Fan role  
so that I can confirm my choice and understand what being a Fan means.

**Acceptance Criteria:**
- AC 1: Page displays "Are you a Fan?" title
- AC 2: Page shows Fan role description and benefits
- AC 3: Page displays relevant Fan icon/illustration
- AC 4: Confirm button is prominently displayed
- AC 5: Navigation back to previous page is available

---

### Task: Handle Fan Role Confirmation

**User Story:**  
As a new user on Fan Role Confirmation Page,  
I want to click the confirm button  
so that I can proceed to set up my email.

**Acceptance Criteria:**
- AC 1: Confirm button click navigates to next step in registration process

---

### Task: Handle Back Navigation from Fan Role Confirmation Page

**User Story:**  
GIVEN user is on Fan Role Confirmation Page,  
As a new user,  
I want to click the back button  
so that I can return to the Choose Role Page.

**Acceptance Criteria:**
- AC 1: Back button is visible and accessible
- AC 2: Back button click navigates to Choose Role Page
- AC 3: Previous role selection state is maintained

---

## Page: Set Username

### Task: Create Set Username Page UI

**User Story:**  
GIVEN user completes Fan Role Confirmation,  
As a new user,  
I want to see a username setup page  
so that I can create a unique username for my account.

**Acceptance Criteria:**
- AC 1: Page displays "Set Your Username" title
- AC 2: Username input field is prominently displayed
- AC 3: Username validation feedback is shown in real-time
- AC 4: Continue button is available when username is valid
- AC 5: Navigation back to previous page is available

---

### Task: Handle Username Input Validation

**User Story:**  
As a new user on Set Username Page,  
I want to see real-time validation of my username  
so that I know if my chosen username is available and meets requirements.

**Acceptance Criteria:**
- AC 1: Username must be at least 3 characters long
- AC 2: Username must be unique (not already taken)
- AC 3: Username can only contain letters, numbers, and underscores
- AC 4: Real-time feedback shows availability status
- AC 5: Error messages are clear and helpful

---

### Task: Handle Continue Button from Set Username Page

**User Story:**  
As a new user on Set Username Page,  
I want to click the continue button with a valid username  
so that I can proceed to complete my account setup.

**Acceptance Criteria:**
- AC 1: Continue button is only enabled when username is valid
- AC 2: Button click saves username to user profile
- AC 3: Button click navigates to next step in onboarding process

---

### Task: Handle Back Navigation from Set Username Page

**User Story:**  
GIVEN user is on Set Username Page,  
As a new user,  
I want to click the back button  
so that I can return to the Fan Role Confirmation Page.

**Acceptance Criteria:**
- AC 1: Back button is visible and accessible
- AC 2: Back button click navigates to Fan Role Confirmation Page
- AC 3: Previous username input state is cleared
- AC 4: Navigation maintains user's role selection context

---

## Page: Set Password

### Task: Create Set Password Page UI

**User Story:**  
GIVEN user completes Set Username,  
As a new user,  
I want to see a password setup page  
so that I can create a secure password for my account.

**Acceptance Criteria:**
- AC 1: Page displays "Create Account" title
- AC 2: Password input field with placeholder "Enter password" is displayed
- AC 3: Password requirements text is shown below input field
- AC 4: Eye icon for show/hide password functionality is visible
- AC 5: Next button is prominently displayed
- AC 6: Navigation back to previous page is available

---

### Task: Handle Password Input Validation

**User Story:**  
As a new user on Set Password Page,  
I want to see real-time validation of my password  
so that I know if my password meets security requirements.

**Acceptance Criteria:**
- AC 1: Password must be at least 8 characters long
- AC 2: Password must include uppercase letters
- AC 3: Password must include lowercase letters
- AC 4: Password must include numbers
- AC 5: Password must include symbols
- AC 6: Real-time feedback shows validation status

---

### Task: Handle Password Visibility Toggle

**User Story:**  
As a new user on Set Password Page,  
I want to toggle password visibility  
so that I can verify what I'm typing.

**Acceptance Criteria:**
- AC 1: Eye icon is clickable and responsive
- AC 2: Clicking eye icon shows password in plain text
- AC 3: Clicking eye icon again hides password
- AC 4: Icon changes state to indicate current visibility mode

---

### Task: Handle Password Error States

**User Story:**  
As a new user on Set Password Page,  
I want to see clear error feedback  
so that I understand what needs to be corrected in my password.

**Acceptance Criteria:**
- AC 1: Input field shows red border when password is invalid
- AC 2: Specific error messages are displayed for each validation rule
- AC 3: Error messages are clear and actionable
- AC 4: Error state is cleared when password becomes valid

---

### Task: Handle Next Button Click from Set Password Page

**User Story:**  
As a new user on Set Password Page,  
I want to click the next button with a valid password  
so that I can proceed to set up my account details.

**Acceptance Criteria:**
- AC 1: Next button is only enabled when password is valid
- AC 2: Button click saves password securely
- AC 3: Button click navigates to Set Account page
- AC 4: Loading state is shown during navigation

---

### Task: Handle Back Navigation from Set Password Page

**User Story:**  
GIVEN user is on Set Password Page,  
As a new user,  
I want to click the back button  
so that I can return to the Set Username Page.

**Acceptance Criteria:**
- AC 1: Back button is visible and accessible
- AC 2: Back button click navigates to Set Username Page
- AC 3: Previous password input state is cleared for security
- AC 4: Navigation maintains user's username and role selection context

---
