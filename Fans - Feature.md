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

## Page: Set Email

### Task: Create Set Email Page UI

**User Story:**  
GIVEN user completes Fan Role Confirmation,  
As a new user,  
I want to see an email setup page  
so that I can enter my email address for my account.

**Acceptance Criteria:**
- AC 1: Page displays "Create Account" title
- AC 2: Email input field with placeholder "Enter your email" is prominently displayed
- AC 3: Next button is available at the bottom of the page
- AC 4: Navigation back to previous page is available
- AC 5: Page follows dark theme design as shown in mockup

---

### Task: Handle Email Input Validation

**User Story:**  
As a new user on Set Email Page,  
I want to see validation of my email address  
so that I know if my email format is correct and available.

**Acceptance Criteria:**
- AC 1: Email must follow valid email format (contains @ and domain)
- AC 2: Email validation occurs on input blur or form submission
- AC 3: Valid email enables the Next button
- AC 4: Invalid email shows appropriate error feedback
- AC 5: Email availability is checked against existing accounts

---

### Task: Handle Email Error States

**User Story:**  
As a new user on Set Email Page,  
I want to see clear error feedback  
so that I understand what needs to be corrected with my email input.

**Acceptance Criteria:**
- AC 1: Input field shows red border when email is invalid
- AC 2: Error message "Please enter a valid email address" is displayed for invalid format
- AC 3: Error message "This email is already connected to a songcry account" is shown for existing emails
- AC 4: Blue "Check ticket link here" link is displayed for existing account errors
- AC 5: Error state is cleared when email becomes valid

---

### Task: Handle Next Button Click from Set Email Page

**User Story:**  
As a new user on Set Email Page,  
I want to click the next button with a valid email  
so that I can proceed to set up my password.

**Acceptance Criteria:**
- AC 1: Next button is only enabled when email is valid and available
- AC 2: Button click saves email to user profile
- AC 3: Button click navigates to Set Password page
- AC 4: Loading state is shown during navigation

---

### Task: Handle Back Navigation from Set Email Page

**User Story:**  
GIVEN user is on Set Email Page,  
As a new user,  
I want to click the back button  
so that I can return to the Fan Role Confirmation Page.

**Acceptance Criteria:**
- AC 1: Back button is visible and accessible
- AC 2: Back button click navigates to Fan Role Confirmation Page
- AC 3: Previous email input state is maintained
- AC 4: Navigation maintains user's role selection context

---

### Task: Create Email Validation API Endpoint

**User Story:**  
As a backend developer,  
I want to create an API endpoint for email validation  
so that the frontend can validate email format and check for duplicates during user registration.

**Acceptance Criteria:**
- AC 1: Create POST endpoint `/api/auth/validate-email` for email validation
- AC 2: Endpoint validates email format using proper regex pattern
- AC 3: Endpoint checks for duplicate emails in the database
- AC 4: Return HTTP 200 status code for valid and available emails
- AC 5: Return HTTP 400 status code for invalid email format
- AC 6: Return HTTP 409 status code for emails that already exist
- AC 7: Response includes JSON format with validation status and error messages
- AC 8: Implement proper error handling for database connection issues

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
so that I can return to the Set Email Page.

**Acceptance Criteria:**
- AC 1: Back button is visible and accessible
- AC 2: Back button click navigates to Set Email Page
- AC 3: Previous password input state is cleared for security
- AC 4: Navigation maintains user's previous input context

---

## Page: Set Username

### Task: Create Set Username Page UI

**User Story:**  
GIVEN user completes Set Password Page,  
As a new user,  
I want to see a username setup page  
so that I can create a unique username for my account.

**Acceptance Criteria:**
- AC 1: Page displays "Create Account" header with back button
- AC 2: Profile picture upload section with placeholder and '+' button is displayed
- AC 3: Username input field with placeholder "Enter your username" is prominently displayed
- AC 4: Informational text about username visibility is shown
- AC 5: Terms of Use and Privacy Policy links are available
- AC 6: Marketing consent checkbox is displayed
- AC 7: "Create Account" button is available at the bottom
- AC 8: Page follows dark theme design as shown in mockup

---

### Task: Handle Username Input Validation

**User Story:**  
As a new user on Set Username Page,  
I want to see real-time validation of my username  
so that I know if my username is available and meets requirements.

**Acceptance Criteria:**
- AC 1: Username must be at least 3 characters long
- AC 2: Username must not exceed 20 characters
- AC 3: Username can only contain letters, numbers, and underscores
- AC 4: Username must be unique (not already taken)
- AC 5: Real-time validation occurs on input change
- AC 6: Valid username enables the Create Account button
- AC 7: Username availability is checked against existing accounts

---

### Task: Handle Username Error States

**User Story:**  
As a new user on Set Username Page,  
I want to see clear error feedback for username issues  
so that I understand what needs to be corrected.

**Acceptance Criteria:**
- AC 1: Input field shows red border when username is invalid
- AC 2: Error message "Username is already taken" for existing usernames
- AC 3: Error message "Username contains inappropriate words" for blocked content
- AC 4: Error message "Username can only contain letters, numbers, and underscores" for invalid characters
- AC 5: Username suggestions are provided when username is taken
- AC 6: Error states clear when username becomes valid

---

### Task: Handle Profile Picture Upload

**User Story:**  
As a new user on Set Username Page,  
I want to upload a profile picture  
so that I can personalize my account.

**Acceptance Criteria:**
- AC 1: Profile picture placeholder is displayed with '+' button
- AC 2: Clicking '+' button opens file selection dialog
- AC 3: Only image files (jpg, png, gif) are accepted
- AC 4: Image preview is shown after selection
- AC 5: File size limit of 5MB is enforced
- AC 6: Error message for invalid file types or size

---

### Task: Handle Terms and Privacy Consent

**User Story:**  
As a new user on Set Username Page,  
I want to review and accept terms and privacy policy  
so that I can complete my account creation.

**Acceptance Criteria:**
- AC 1: "Terms of Use" link opens terms document
- AC 2: "Privacy Policy" link opens privacy document
- AC 3: Marketing consent checkbox is optional
- AC 4: Links open in new tab/window
- AC 5: Consent state is tracked for account creation

---

### Task: Handle Create Account Button Click

**User Story:**  
As a new user on Set Username Page,  
I want to click Create Account with valid inputs  
so that I can proceed to set my date of birth.

**Acceptance Criteria:**
- AC 1: Create Account button is only enabled when username is valid
- AC 2: Button click saves username and profile picture
- AC 3: Button click navigates to Set Date of Birth page
- AC 4: Loading state with spinner is shown during processing
- AC 5: Error handling for account creation failures

---

### Task: Handle Back Navigation from Set Username Page

**User Story:**  
GIVEN user is on Set Username Page,  
As a new user,  
I want to click the back button  
so that I can return to the Set Password Page.

**Acceptance Criteria:**
- AC 1: Back button is visible and accessible
- AC 2: Back button click navigates to Set Password Page
- AC 3: Previous username input state is maintained
- AC 4: Profile picture selection is preserved
- AC 5: Navigation maintains user's previous input context

---

### Task: Handle Username Loading States

**User Story:**  
As a new user on Set Username Page,  
I want to see loading indicators during username validation  
so that I know the system is processing my input.

**Acceptance Criteria:**
- AC 1: Loading spinner appears during username availability check
- AC 2: Input field shows loading state during validation
- AC 3: Create Account button shows loading state during submission
- AC 4: Loading states prevent multiple simultaneous requests
- AC 5: Timeout handling for slow network responses

---

### Task: Create Username Validation API Endpoint

**User Story:**  
As a backend developer,  
I want to create an API endpoint for username validation  
so that the frontend can validate username availability and format during user registration.

**Acceptance Criteria:**
- AC 1: Create POST endpoint `/api/auth/validate-username` for username validation
- AC 2: Endpoint validates username format (3-20 chars, alphanumeric + underscore)
- AC 3: Endpoint checks for duplicate usernames in the database
- AC 4: Endpoint filters inappropriate words using content moderation
- AC 5: Return HTTP 200 status code for valid and available usernames
- AC 6: Return HTTP 400 status code for invalid username format
- AC 7: Return HTTP 409 status code for usernames that already exist
- AC 8: Response includes JSON format with validation status, error messages, and username suggestions
- AC 9: Implement proper error handling for database connection issues
- AC 10: Rate limiting to prevent username enumeration attacks

---

### Task: Create Profile Picture Upload API Endpoint

**User Story:**  
As a backend developer,  
I want to create an API endpoint for profile picture upload  
so that users can upload and store their profile images during registration.

**Acceptance Criteria:**
- AC 1: Create POST endpoint `/api/auth/upload-profile-picture` for image upload
- AC 2: Endpoint accepts multipart/form-data with image file
- AC 3: Validate file type (jpg, png, gif) and size (max 5MB)
- AC 4: Generate unique filename to prevent conflicts
- AC 5: Store image in secure cloud storage or local directory
- AC 6: Return HTTP 200 with image URL for successful uploads
- AC 7: Return HTTP 400 for invalid file type or size
- AC 8: Implement image optimization and resizing
- AC 9: Proper error handling for storage failures
- AC 10: Security measures to prevent malicious file uploads

---
