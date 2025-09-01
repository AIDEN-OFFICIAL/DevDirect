
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
3. ID Verification (optional) (build truds twith a varified badge )
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

### 5. Student Journey

#### Dashboard
- **Upcoming Session** (Rect card)  
  - Interviewer name + photo (top, left)
  - Domain (stu selected)  
  - Timer (enabled before 15 min, left down)  
  - Prep sheet button (modal, icon:paper)  
  - Chat button (modal, icon: message, right to prep sheet)  
  - Join session (enabled 3 min before start)  
- **Booking History**  (All Upcoming sessions)
  - Grid of session cards  (four column)
  - Color cues: green=accepted, red/gray=pending  
  - Modal: detailed session info + chat option (This looks like the first card with all the details)
- **Past Sessions**  
  - List in chronological order  
  - Shows interviewer, date, time, star rating  
  - Click → summary + notes (Pendings)

---


