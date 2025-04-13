# Reelrz Pages

## General Pages (Accessible to All Users)

### Homepage
- Purpose: Introduces the platform, highlights its value, and may feature popular job offers, top freelancers, or a call-to-action for registration/login.
- Key Elements: Sign-up/login buttons, brief platform overview, and possibly a search bar.
### Registration Page:
- Purpose: Allows new users to sign up as either a freelancer or brand owner.
- Fields: First name, last name, email, phone number, country, region, gender, birthday, account type (freelancer/brand owner), account image (optional), and social login options (provider/provider_id).
- Post-Submission: Email/phone verification step.
### Terms of Service, Privacy Policy, About Us:
- Purpose: Static pages for legal and informational content.

-----
## Freelancer-Specific Pages

### Freelancer Dashboard:
- Purpose: Central hub post-login.
- Features: 
    - all jobs with filter(recommended, ongoing, cancelled, and completed jobs)
    - earnings summary
    - quick links to profile
    - messages (all chats)
    - notifications.
    - all projects (portfolio)
    - Balance and Transaction History Page
    - freelancer  information
        - personal info 
        - Bio
        - specialization
        - job title
        - skills
    - add new project to portfolio (can use same structure to project edit page)
        - title
        - description
        - thumbnail (image upload)
        - skills
        - category
        - video link from PROJECTS

### Freelancer Profile View Page:
 Publicly viewable profile showcasing their:
    - details (about freelancer)
    - skills
    - portfolio(projects)
    - rating and reviews

### Job Offer Listing Page:
- Purpose: Browse and search available job offers.
- Features:
    - Filters (e.g., category, budget, deadline),
    - search bar
    - job cards with 
        - thumbnail
        - title
        - description
        - budget 
        - required skills.
        - report button for report this job offer (it will be modal)

### Job Offer Details Page:
- Purpose: View full details of a job offer and submit a proposal.
- Content:
    - Title
    - description
    - budget
    - required 
    - skills
    - deadline
    - brand owner details
    - "Submit Proposal" button.
    - list of all submitted proposals with its details
        - name of freelancer 
        - part of cover latter
        - report button for report this proposal (it will be modal)
### Proposal Submission Page:
- Purpose: Submit a proposal for a job offer.
- content:
    - Cover letter
    - proposed price
    - estimated delivery
    - attachments

  **Note:** This can be implemented as a modal dialog overlay instead of a separate page to provide a seamless user experience without requiring navigation away from the job offer details.

-----
## Brand Owner-Specific Pages

### Brand Owner Dashboard:
- Purpose: Central hub post-login.
- content: 
    - Posted job offers
        with status (, in_progress, completed, cancelled)
    - received proposals
    - ongoing jobs
    - messages (all chats)
    - notifications.
    - Balance and Transaction History Page 
    - Brand Owner  information
        - personal info 
### Brand Owner Profile View Page:
Purpose: Publicly viewable profile showcasing their company details and its last projects 

### Job Offer Creation Page:
Post a new job offer with :
    - Title
    - description
    - budget
    - link
    - required
    - skills
    - deadline
## Shared Pages (Freelancers and Brand Owners)
### Chatting page 
that show all job offers chats for freelancer and brand owner with their job offer 

### Deposit Page
- Purpose: Add funds to the account.
-  Features: Payment method selection (bank card, mobile wallet), amount input, secure payment gateway integration.

### Withdrawal Page:
- Purpose: Request earnings withdrawal.
- Fields: Amount, destination type (bank/mobile wallet), destination details, status tracking (pending, approved, failed).

### Rating and Review Submission Page 
it will be modal 
- Ratings (1-5) for
    -  recommend_to_others
    -  professionalism
    -  communication
    -  quality
    -  expertise
    -  deadline respect
    - willingness to work again
- review text

