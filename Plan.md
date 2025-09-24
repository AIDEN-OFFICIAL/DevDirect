
# DevDirect - Project Planning
## _DevDirect: Your career, accelerated_

DevDirect is a platform for aspiring developers to practice interviews with experienced professionals.  
It helps you prepare for your dream job by providing direct access to industry insights and targeted feedback.   

---

## 🧠 Ideas
**[**
- **Interviewer Profile Setup**  
  When an interviewer creates their profile, they'll specify their domain and expertise levels in different technologies.

- **Student Questionnaire**  
  After a student books an interview slot, they'll fill out a questionnaire detailing their experience, desired topics, and any specific questions they have.

- **Interview Preparation**  
  The interviewer receives the student's questionnaire and uses it to prepare for the session.
**]**

---

## 🌐 Application Pages

### 1. Homepage

**Goal:**  
The goal of the homepage is to clearly and quickly explain what DevDirect is and guide both students and interviewers to their respective journeys. The design should be clean, professional, and easy to navigate.

This is a great approach. Breaking the project down into individual pages and focusing on one at a time will make the process much more manageable.  
Let's start with the very beginning: the Homepage. This is the first page a user sees, and its design sets the entire tone for the platform.

**Sections:**

1. **Navigation Bar (Top)**  
   - Logo (Left)  
   - Navlinks: "How It Works," "For Students," "For Interviewers," and "About Us."  
   - Login (clr: simple) & Sign-Up Buttons (clr: prominent, far Right)  

2. **Hero Section (Below the Navigation Bar)**  
   - Heading: (Motto)  
   - Sub-heading  
   - Button1: "I’m a Student"  
   - Button2: "I’m an Interviewer"  
   - [Clicking on either button → leads to a separate login page. Even if they click Login/Signup, if they are not signed up, they will be given a role selection checkbox first. Only one database will be used; roles will be assigned.]  

3. **Features Section**  
   - **Headings**: ("Why DevDirect?" or "How It Works.")  
   - **Layout**: three-section vertical layout (3 cols)  
     - Sec1: Expert Interviewers (Icon: professional looking, tie/briefcase. Title: *Practice with the Pros*. Desc: "Our interviewers are real professionals from leading tech companies, verified to ensure you get the most accurate and up-to-date industry feedback.")  
     - Sec2: Flexible & Convenient (Icon: calendar/clock. Title: *Book when it works for you*. Desc: "Find and book mock interviews that fit your schedule. With a wide range of professionals available, you can practice on your own time, from anywhere.")  
     - Sec3: Targeted Growth (Icon: rocket/uptrend. Title: *Accelerate Your Career*. Desc: "Receive personalized, actionable feedback after every session. Our interviewers help you identify weak points and build the confidence you need to ace your real job interview.")  
     - Sec4: Specialized Courses (Icon: book/diploma. Desc: "Beyond mock interviews, access a library of specialized courses and content designed by our expert interviewers to fill any gaps in your knowledge.")  

4. **For Interviewers Section**  
   - Heading: *For Interviewers: Monetize Your Expertise* (bold)  
   - Sub-heading: "Your skills are in demand. Join our platform to share your knowledge and earn on your own terms."  
   - Content:  
     1. Set Your Own Price  ( You're in control of your earnings. You can set the price that you feel your time and expertise are worth.)
     2. Flexible Scheduling (List your available hours and take interviews when it works for you. No long-term commitment.
)
     3. Make an Impact (Help the next generation of developers land their dream jobs and build a community around your expertise.)  
   - CTA: *Become an Interviewer*  

5. **Description Section**  
   - "Find Your Match": Highlights filtering to find perfect interviewers.  
   - "Get Real-World Practice": Benefits of mock interviews.  
   - "Build Confidence": Focus on soft skills + confidence gained.  

6. **Testimonials**  
   - "Hear from users" → display ratings and feedback.  

7. **Footer**  
   - Links: "About Us," "Contact," "Privacy Policy," "Terms of Service."  
   - Social media + trademarks  

---

### 2. Authentication
  [Main contentainer: Centered ]
#### Sign-Up Page
- Heading: "Join DevDirect."  
- Role selection: (radio → Student | Interviewer)  
- Input: Email, Password, Confirm Password  
- Submit: Sign Up  
- Link: Already have account? → Login  

#### OTP Verification
- Heading: Verify email address  
- Input: numeric only  
- Verify button  
- Resend OTP (appears after 30s, refresh only on click)  

#### Login
- Inputs: Email + Password  

---

### 3. Interviewer Journey

#### Profile Setup
1. Personal Info: Pic, Name, Job Title, Company, Bio  
2. Expertise & Domains 

  Button:(clicks to reveal a new section to input a domain.)
   - Add domain(s)  
   - Skills (drop down to select from) + Expertise levels (Beginner → Expert)  
3. ID Verification (optional) (build trust with a varified badge )
4. CTA: Submit & Proceed to Test  

#### Test Landing Page
**Heading:**  
"Verify Your Expertise."  

**Informational Text:**  
"To ensure the quality and credibility of our platform, all interviewers must complete a brief technical assessment. This test helps us match you with the right students and builds trust with our community. You can start the test whenever you feel ready."  

**Design Goal:**  
This page's design should be simple and focused on encouraging the interviewer to begin the test when they're ready. The layout gives the interviewer a clear message and puts them in control.  

**Elements:**  
- Prominent heading at the top ("Verify Your Expertise.")  
- Encouraging paragraph below  
- Large central button: *Start Test* (only CTA on the page, eye-catching, centered)  

**Flow:**  
- Once the interviewer clicks *Start Test*, they are taken to the assessment where pre-built questions are presented one by one.  

---

#### Test Page
- Central chat window (Q&A style)  
- Progress bar + status (Q3 of 10)  
- Timer (10 mins and decreasing, top-center)  
- Input field + send button  (right down)

#### Test Results Page
- **If Pass**  
  - Heading: Congratulations  
  - Message: Welcome, verified  
  - Body: Welcome message ("Your expertise has been verified. You can now set up your availability and start taking mock interviews on DevDirect!")
  - Input: Set hourly rate (default 50, editable)  
  - Button: Go to Dashboard (redirect to dashboard)
 
- **If Fail**  
  - Heading: Review Results  
  - Message: Didn’t meet threshold  
  - Try again → disabled for 24 hrs (You can retake the test in 24 hours
)  

---

### 4. Interviewer Dashboard

#### Layout
- **Left Column (Quick Stats)**  
  - Upcoming bookings (details (name, session time), countdown (disabled before 15min), join button (enabled before 3mins), chat option)  
  - Total earnings (clickable → earnings page)  
  - Average ratings (clickable → reviews page)  
- **Right Column (Recent Activity)**  
  - Notifications: new bookings, reviews, payments, messages  
- Links: Edit Profile, etc.  

#### Schedule & Availability (lot booking)
- Weekly recurring schedule [select hours (list of time slots : (e.g., 5-6 AM, 6-7 AM) ) + days (M, T, W...)]
- Vacation mode toggle  (disable all slots)

#### Bookings & Sessions
1. Pending requests (list view scrollable cards, 45 mins to accept, accept/decline buttons) <each card: name , req date and time , countdown timer only 45 mins to accept each card will have accept and decline buttons> 
2. Upcoming sessions (accepted sessions chronological : <name, sess date and time, domain >)
3. Past sessions (list view scrollable, with rating + feedback tabs click to view : student’s feedback (modal), interviewer’s notes)  
[ modal:
**tab1**:students feedback
 			overall ratings
 			written review: feedback

**tab2**: Interviewers ' notes (Your notes):
 			PENDINGS given]

#### Earnings & Payouts
- **Summary**: withdrawable (large font), total earnings (smaller on the corner), pending payouts (payment done on the very nxt day) 
- **History**: date, description, status, amount  

#### Profile Management
- Profile status toggle (live/paused)  
- Public profile: Pic, Name, Bio, Title, Expertise tags  
- Hourly rate (editable, shows fee deduction)  
- Account & security: Email, Password, 2FA, Delete account  
- Save changes button appears when edits made  

#### Ratings & Reviews
- Overall rating + breakdown (hw many stars)
- List of reviews (student comments, dates)  
- Optional: public interviewer reply feature  

#### Notifications History
- Filters: All | Unread (another shade) | Messages( from stu, icon:message) | Alerts (icon: bell, all types eg: payment, rev left etc...)
- Chronological list (icon, sender/title, timestamp, unread shading)  

---

# 📘 Student Journey (Complete – All Notes Preserved)

---

## 1. Student Dashboard

### Upcoming Session (Primary)
- Rectangular card, fixed at the top of the dashboard.  
- **Contents**:  
  - Interviewer’s name + profile picture (top-left).  
  - Domain selected for interview.  
  - Countdown timer (top-right; disabled by default, enabled 15 min before session start).  
  - Buttons (bottom row, left → right):  
    - **Prep Sheet button** (paper icon; opens modal styled like notebook page).  
    - **Chat button** (message icon; opens modal; placed right of prep sheet).  
    - **Join Session button** (enabled only 3 min before start).  

### Booking History
- Heading: “All Upcoming Sessions”.  
- Rectangular cards displayed in a 4-column grid.  
- **Border color codes**:  
  - Green = accepted.  
  - Red/Grey = pending.  
- **Card details**: serial number, date & time, domain booked.  
- **On click (modal)**: shows interviewer name, date & time, chat option, layout same as upcoming session card.  

### Past Sessions
- Chronological list of completed sessions.  
- **Summary card**: interviewer name, date, time, star rating.  
- **On click (modal)**: session summary + interviewer notes (pending topics, overall feedback).  
- **Top-left counter**: displays total number of sessions completed.  

---

## 2. Interviewer Search Page

### Search & Filter
- Search bar fixed at the top.  
- Filter panel accessible via hamburger icon (top-right).  
- **Filter options**:  
  - Availability (show only green-bordered cards, or select specific date/time).  
  - Price range (slider with min–max).  
  - Expertise (filter by skill tags).  
  - Years of experience (slider/dropdown).  

### Interviewer Cards (Rectangular)
- **Top-left**: profile picture (medium circle).  
- **Right of photo**: name + title (e.g., “Senior Software Engineer”).  
- **Below name**: 2–3 expertise tags displayed as chips.  
- **Top-right**: average rating (stars).  
- **Bottom-right**: hourly rate.  
- **Bottom-center CTA**: *View Profile*.  
- **Border states**:  
  - Green = available now.  
  - Red = currently in session (status text shown, e.g., “In session until 6:00 PM”).  
  - Grey = offline.  

---

## 3. Interviewer Profile Page

### Top Section (Two-Column Layout)
- **Left column (Profile Block)**:  
  - Profile picture (top-left, large circle).  
  - Name & title (below photo, bold).  
  - Rating (stars + review count, inline row).  
  - Hourly rate (bottom, right-aligned small text).  

- **Right column (Booking Block)**:  
  - Dynamic CTA button (top-right, above calendar):  
    - Green = “Book Now” (direct booking + payment).  
    - Red = “Request a Session” (future slot selection via modal).  
    - Grey = “Not Accepting Bookings” (disabled).  
  - Availability calendar (center-right, full width; shows slots in student’s local timezone).  

### Main Section (Single Column, full width below top section)
- About Me (bio).  
- Skills & Expertise (tags/rows).  
- Reviews (chronological, list of student feedback).  

---

## 4. Booking & Payments Page

### Step 1: Order Summary
- Interviewer name + profile picture (top-left, small circle).  
- Date & time (below name, includes weekday).  
- Domain selected.  
- Pricing breakdown (right column):  
  - Hourly rate.  
  - Platform fee.  
  - Taxes.  
  - **Final total (bold)**.  

### Step 2: Payment & Prep Notes
1. **Preparation Notes Modal**  
   - Triggered by paper icon in booking form.  
   - Modal styled like a notebook page.  
   - Fields:  
     - Domain (text field).  
     - Topics (textarea for listing topics).  
     - Description (multi-line text area for extra context).  

2. **Payment Section**  
   - Credit Card Number.  
   - Expiration Date (MM/YY).  
   - CVV/CVC.  
   - Secure transaction message shown below fields.  

3. **Final CTA Button**  
   - Label: *Pay & Confirm Booking*.  
   - Button enabled only when both prep notes + payment fields are filled.  
   - On success → booking confirmed.  

### Booking System Logic
- **Payment failure**: booking not finalized, slot remains available, student asked to retry.  
- **Simultaneous booking**: slot placed on temporary hold (5–10 min during checkout); auto-released if unpaid.  

### Post-Booking Flow
- **Student**: redirected to booking confirmation page → email confirmation (session details + receipt) → dashboard updated (session appears under *Upcoming Sessions*).  
- **Interviewer**: immediate notification + email alert → dashboard calendar updated (slot marked booked) → upcoming sessions updated → access to student’s prep notes.  

---

## 5. Live Session Page

### Core Components
- Video feed (main area, center, largest portion).  
- Chat box (side panel or bottom-right toggle).  
- Interviewer notes panel (above chat, labeled “Notes & Pending Topics”).  
- Session timer (top-center, countdown).  
- End Session button (top-right, red).  
- No-Show button (appears only after 5-min grace period, placed subtly below or beside end session).  
- **Design goal**: minimal, distraction-free layout.  

### Timer Logic & Feedback Pop-Up
- Timer runs normally.  
- Last 15 minutes → timer turns red.  
- Pop-up: “Feedback Time” → prompts interviewer to start live feedback.  
- Flexible: for shorter sessions (<1hr>), trigger proportional feedback warning.

### Potential Issues & Solutions
- **Connection issues**: auto-switch to audio-only, small alert icon shown.  
- **No-show**: report button becomes available after 5 min grace → triggers support workflow + refund.  

---

## 6. Post-Session Flow & Feedback Forms

### Interviewer Feedback
- Auto-prompted form after session ends.  
- Fields:  
  - Pending topics (pre-populated from notes).  
  - Overall feedback (free text).  
- Stored in student’s feedback record for future prep.  

### Student Feedback
- Auto-prompted form after session ends.  
- Fields:  
  - Star rating.  
  - Suggestions for improvement (free text).  
- Reflected on interviewer’s public profile.  

---

## 7. Reviews & Feedback Page

### Layout
Two main sections:  

1. **Feedback from Interviewers**  
   - Chronological list of cards.  
   - Shows interviewer name + date.  
   - Expandable view → full feedback & pending topics.  

2. **My Reviews**  
   - Chronological list of reviews given by student.  
   - Each shows interviewer name, date, star rating.  
   - Option to edit existing reviews.  

---

## 8. Account Settings Page

### Layout
- Left-hand navigation panel (list of sections).  
- Right-hand main content area displays selected section.  

### Sections
- **Personal Information**: edit name, email, profile photo.  
- **Payment Settings**: add/remove/manage saved credit cards.  
- **Security**: change password, enable two-factor authentication.  
- **Notifications**: checkboxes to toggle email alerts + in-app alerts.  

**Goal**: secure, user-friendly, with all essential settings available.  

---
# 🛠️ Admin Side – DevDirect

The Admin Panel gives platform administrators complete control over **users, content, disputes, analytics, and settings**.  
Layout prioritizes clarity, with a **two-column grid**: navigation sidebar on the left, and content area on the right.

---

## 1. Admin Dashboard

### Layout & Positioning
- **Primary Layout**: two-column grid.  
- **Header**: “DevDirect Admin” (top) + profile icon / Logout button (top-right).  
- **Left Sidebar Navigation**:
  - Dashboard *(homepage of admin panel)*  
  - User Management  
    - Students  
    - Interviewers  
  - Content & Moderation  
    - Reviews  
    - Disputes  
    - Reported Issues  
  - Analytics & Reports  
  - Settings  

### Dashboard Content
- **Quick Stats Section** *(row of prominent cards, top of main content)*:
  - Card 1: **Total Users** (students + interviewers).  
  - Card 2: **Active Sessions** (live interviews currently running).  
  - Card 3: **Platform Earnings** (total revenue over selected time period).  

- **Recent Activity Log** *(below stats cards, left side)*:  
  - Chronological list of sign-ups, bookings, reported issues.  
  - Scrollable feed.  

- **Quick Access Buttons** *(below stats cards, right side)*:  
  - “Manage Users” → opens User Management.  
  - “Review Disputes” → jumps to Dispute Resolution section.  

---

## 2. User Management

### Layout & Positioning
- **Two-tabbed layout** (top of page): *Students* | *Interviewers*.  
- **Search & Filter bar**:  
  - Interviewers: filter by *Verified*, *Pending Verification*, *Suspended*.  
  - Students: filter by *Active*, *Suspended*.  

### 2.1 Interviewer Management
- **Table/Grid Display**: searchable, sortable.  
- **Columns**: Name, Email, Status, Action (verify/reject).  
- **Status Values**: Verified, Pending, Not Submitted.  
- **Verification Flow**:
  - Click on interviewer profile → opens modal/new page.  
  - Modal shows: uploaded ID, proof of work.  
  - **Action Buttons**:  
    - “Verify & Grant Badge” → adds verified badge to public profile.  
    - “Reject” → requires admin to add rejection note (visible to interviewer).  

### 2.2 Student Management
- **Table/Grid Display**: searchable, sortable.  
- **Columns**: Name, Email, Status.  
- **Actions**:
  - Suspend / Activate account.  
  - View student booking history.  

### Summary of Admin Actions
- **Interviewers**: Verify/Reject Profile, Suspend/Activate Account, Edit Public Profile.  
- **Students**: Suspend/Activate Account, View Booking History.  

---

## 3. Content & Moderation

### Layout & Positioning
- **Tabbed interface** at top of content area.  
- Tabs: *Reviews* | *Disputes* | *Reported Issues*.  

### 3.1 Reviews Tab
- **Purpose**: monitor/manage reviews from students.  
- **Display**: searchable, filterable chronological list.  
- **Actions**: Archive or Delete reviews (if policy violation).  

### 3.2 Disputes Tab
- **Purpose**: resolve conflicts (e.g., no-shows, payments).  
- **Display**: open/closed cases list.  
- **Case Details View**:
  - Chat log of session.  
  - Button to access full video recording.  
  - Original complaint text.  
- **Actions**:
  - “Issue Full Refund to Student”.  
  - “Grant Full Payout to Interviewer”.  
  - “Resolve” → partial refund options.  
  - Toggle: *Block Interviewer’s Payout* (system auto-blocks until resolved).  
- **Legal Note**: Booking page must show disclaimer: *all sessions recorded for dispute resolution*.  

### 3.3 Reported Issues Tab
- **Purpose**: queue of user-reported issues (e.g., inappropriate content).  
- **Display**: chronological list of reports.  
- **Actions**: archive issue, suspend user’s account.  

---

## 4. Analytics & Reports

### Layout & Positioning
- **Dashboard-style layout** with multiple widgets.  
- **Top Filters**: date range selector, filters by domain, user type.  

### Core Components
- **Platform Health Overview** *(top)*:
  - User Growth → line chart (new sign-ups over time).  
  - Booking Trends → bar chart (weekly/monthly bookings).  

- **Performance Insights** *(below health overview)*:
  - Top Interviewers → ranked by bookings or average rating.  
  - Popular Domains → pie/bar chart showing in-demand topics.  

- **Revenue Report** *(separate section)*:
  - Total Earnings → card (gross revenue).  
  - Payouts & Fees → breakdown: interviewer payouts vs platform fees.  

---

## 5. Admin Settings

### Layout
- **Left-hand list navigation**, similar to main Admin Panel.  
- **Right-hand content area**: displays settings for selected category.  

### Sections
- **General Settings**:
  - Configure platform name.  
  - Primary contact email.  
  - Toggle: *Maintenance Mode*.  

- **Billing & Payments**:
  - Set platform fee % (field).  
  - Global tax rate (editable text box).  
  - Payout thresholds (set limits before payouts processed).  

- **User Notifications**:
  - Manage automated emails & in-app alerts.  
  - List view of all notifications.  
  - Click on template → edit text + variables.  
