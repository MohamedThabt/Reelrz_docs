## Database Design
DBMS: MYSQL
- and will use central server and scale vertical when number of users increased (100000)
### Modules :
#### 1- users and profiles 
- USERS
- IDENTITY_AUTHENTICATIONS 
- ADMINS
- FREELANCER_PROFILES
- SKILLS
- FREELANCER_SKILLS
- PROJECTS
- BRAND_OWNER_PROFILES
- USER_BANS

#### 2- 

-----



```mermaid
erDiagram
 
    USERS {
        bigint id PK
        string first_name
        string last_name
        string email UK
        string phone_number
        string country
        string region
        string gender
        string account_image
        enum account_type "brand_owner, freelancer"
        date birthday
        boolean verified "true, false"
        string provider "Nullable"
        string provider_id "Nullable"
        timestamp created_at
        timestamp updated_at
    }
    IDENTITY_AUTHENTICATIONS {
        bigint id PK
        bigint user_id FK
        string front_side
        string back_side
        string selfie_with_front_id
        enum status "pending, denied, accepted"
        timestamp created_at
        timestamp updated_at
    }
    ADMINS {
        bigint id PK
        string name
        string email UK
        string password
        enum role "admin, moderator"
        timestamp created_at
        timestamp updated_at
    }
    
    FREELANCER_PROFILES {
        bigint id PK
        bigint user_id FK
        text bio "Nullable"
        string specialization "Nullable"
        string job_title "Nullable"
        timestamp created_at
        timestamp updated_at
    }
    
    SKILLS {
        bigint id PK
        string name
        string category "Nullable"
        timestamp created_at
        timestamp updated_at
    }
    
    FREELANCER_SKILLS {
        bigint freelancer_profile_id FK
        bigint skill_id FK
        int proficiency_level "Nullable"
        timestamp created_at
        timestamp updated_at
    }

    PROJECTS {
        bigint id PK
        bigint freelancer_profile_id FK
        string title
        text description
        string thumbnail
        string image
        json skills
        string category
        string link
        timestamp created_at
        timestamp updated_at
    }

    BRAND_OWNER_PROFILES {
        bigint id PK
        bigint user_id FK
        string company_name
        string industry
        string website "Nullable"
        text description "Nullable"
        timestamp created_at
        timestamp updated_at
        }

    USER_BANS {
        bigint id PK
        bigint user_id FK
        bigint banned_by FK "References ADMINS.id"
        timestamp expires_at "Nullable"
        text reason "Nullable"
        int times_banned
        timestamp created_at
        timestamp updated_at
        }

    USERS ||--o{ IDENTITY_AUTHENTICATIONS : has
    USERS ||--o| FREELANCER_PROFILES : has
    FREELANCER_PROFILES ||--o{ FREELANCER_SKILLS : has
    SKILLS ||--o{ FREELANCER_SKILLS : included_in
    FREELANCER_PROFILES ||--o{ PROJECTS : has
    USERS ||--o| BRAND_OWNER_PROFILES : has
    ADMINS ||--o{ USER_BANS : issued_by
    USERS ||--o{ USER_BANS : has
```