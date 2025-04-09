## Authentication and Profile

- **Easy Register and Login**
  - Sign up or log in using Google or Facebook.
  - Integration with **Laravel Socialite** for social login.

- **User Information**
  - First Name
  - Last Name
  - Email
  - Phone Number
  - Country
  - Region
  - Gender
  - Account Image
  - Account Type:
    - Creator / Influencer
    - Brand Owner
- verified (true ,false )
- **Identity Authentication**
  - Front Side
  - Back Side
  - Selfie with Front ID
  - Accepted status (indicates successful verification).

- **Creator Portfolio**
  - Each creator or influencer (freelancer) must have a profile with at least 3 projects to qualify for brand projects.
  - Each project includes:
    - Project Title
    - Project Description
    - Project Thumbnail
    - Project Image
    - Related Skills (Menu and input tag for skills)
    - Project Category
    - Project Link
- brand owner profile 
	- name, industry, and website, as it describes the entity rather than a collection of work samples.

- **User Profile Page**
  - Personal Information
  - All Projects
  - Ratings and Reviews

- **User Settings Page**
  - Edit Personal Information
  - Reset Password
  - Edit Portfolio Projects
- Banned user list 
	- user banned reason
	- who banned user 
	- 3 times of band and after that user account is deleted 
	- the banned prevent user from post project (if he business owner ) or add proposal (if he freelancer) for 1 month
---

## Real-Time Search and Filtration

Applicable on Creator/Influencer and Brand Projects Pages.

- **Filters**
  - Region
  - Price
  - Project Category (e.g., UGC, Storytelling, etc.)
  - Skills
  - General Search

---

## Chatting System

- **Chat Activation**
  - Chat opens only when a brand owner accepts a creator's proposal.
  
- **Message Restrictions**
  - Messages cannot be edited or deleted after being sent.
  - Users can send files, images, and videos.
  - Voice notes are also supported.

- **Admin Monitoring**
  - Admins can read all chats to ensure compliance with platform rules.

---

## Ratings and Reviews

- **After Project Completion**
  - Brand owners can rate and review creators.
  - Ratings and reviews are displayed in the creator’s portfolio.
  - Creators are ranked based on their ratings.

---

## Payment and Commission

- **User Balance**
  - Each user has a **balance** in their account.
  - Users can **charge** their balance or **withdraw** funds using:
    - Mobile Wallets
    - Bank Cards (via Paymob or Fawaterk integration)

- **Brand Owner Requirements**
  - Brand owners must charge their balance before hiring a creator.
  - **Platform Commission**: 20% of the total project value.

---

## Brand Owner Projects System

- **Project Details**
  - **Title**: Short, clear name of the project.
  - **Description**: Detailed explanation of the work needed, goals, and expectations.
  - **Category**: Defines the type of work (e.g., UGC, Storytelling, etc.).
  - **Skills Required**: Lists relevant skills (e.g., Montage, etc.).
  - **Budget**: Fixed price or hourly rate.
  - **Deadline**: Project timeline or delivery date.

- **Client-Side Features**
  - Create and post projects.
  - Browse creator profiles and invite bids.
  - View proposals and select a creator.
  - Communicate via built-in chat.
  - Fund the project by charging the balance.
  - Request revisions, approve work, or close the project.
  - Rate and review creators after completion.

- **Creator-Side Features**
  - View available projects and submit proposals.
  - Proposals include price, timeline, and message.
  - Accept or decline invitations.
  - Start work after selection and submit deliverables.
  - Communicate directly with the client.
  - Receive milestones or full payment upon approval.
  - Withdraw earnings after completion.

- **Payment & Commission**
  - Client funds the project (escrow).
  - Platform deducts a **20% commission** from the creator's earnings.
  - **Creator receives 80%** of the project amount.
  - Payout methods: PayPal, bank transfer, mobile wallet, or other methods.

- **Project Statuses**
  - **Open**: Accepting proposals.
  - **In Progress**: Creator selected, work started.
  - **Under Review**: Work submitted, client reviewing.
  - **Completed**: Work approved, payment released.
  - **Cancelled**: Project stopped by client or creator.

- **Safety & Dispute Resolution**
  - Escrow system ensures secure payments.
  - Dispute resolution team available for conflicts.

---

## Notification System

### **1. Notification Channels**
- **In-app Notifications**: Displayed via a bell icon 🔔 (top bar).
- **Email Notifications**: For important events such as project awarded, payment released, etc.

### **2. Notification Events**
#### 🧑‍💼 **User Activity**
- Account created / welcome notification
- Balance updates (charged, withdrawn, or credited)
- Profile updates or approval

#### 📂 **Project Activity**
- Project posted
- Proposal received
- Proposal accepted/rejected
- Project awarded
- Work submitted
- Revisions requested
- Project marked as completed
- Project canceled

#### 💬 **Messages**
- New message received
- Message reply received

#### 💰 **Payments**
- Payment received
- Commission deducted (e.g., 20%)
- Withdrawal requested/approved

---

## Admin Dashboard – Full Feature Overview

### **1. Dashboard Overview**
- **Summary Widgets**:
  - Total users (Brand Owners & Creators)
  - Active projects
  - Completed projects
  - Total revenue (platform earnings after commission)
  - Pending withdrawal requests
- **Recent Activity Feed**: User signups, project creation, latest transactions.
- **Quick Actions**: Approve users, resolve disputes, send announcements.

### **2. User Management**
- View all users (filter by type: Brand owner / creator)
- Search, sort, and filter by registration date, activity, status
- View user profiles and project history
- Edit, ban, or delete accounts
- Verify or approve identity authentication

### **3. Project Management**
- View all posted projects
- Filter by category, status (open, in progress, completed, cancelled)
- View project details, participants, budget
- Manually intervene (e.g., cancel a project, assign a creator)

### **4. Proposal Management**
- View submitted proposals
- Filter by project, creator, or brand owner
- Approve, reject, or flag suspicious proposals

### **5. Payment & Commission Management**
- View platform earnings (with date filtering)
- Track commission per project (e.g., 20% from creators)
- Manual adjustment of commission rate (per user or project)
- Payment logs: balance charges, withdrawals, and transfers
- Approve or decline withdrawal requests
- View payment gateway logs (Paymob, Fawaterk)

### **6. Notification Center**
- View all system notifications
- Send global or targeted notifications to users
- Edit templates for in-app/email messages

### **7. Messaging & Reports**
- View flagged messages
- Handle user-reported issues (spam, abuse, fraud)
- Internal chat log viewer (for moderation)

### **8. Analytics & Insights**
- Platform usage trends (daily/weekly/monthly)
- Top clients and top creators
- Project category distribution
- Payment volume trends

### **9. Support & Dispute Resolution**
- View open disputes
- Chat history between users involved in disputes
- Make decisions: approve refund, mediate, block users

### **10. System Settings**
- Manage categories, skills, and tags
- Commission rates configuration
- Email & notification settings
- Payment gateway credentials (Paymob, Fawaterk)
- Maintenance mode toggle

### **11. Content & CMS Management**
- Manage landing page content
- Add/update FAQ, terms of service, privacy policy
- Blog or announcement system (optional)

``
