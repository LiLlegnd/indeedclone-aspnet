# IndeedClone - ASP.NET MVC Project  (HMVC)

IndeedClone is a job portal web application inspired by Indeed.  
It allows recruiters to post jobs and candidates to browse and apply for jobs.

## Folder Structure


```text
.
└── IndeedClone
    ├── Emails
    │
    ├── Modules (Modular architecture)
    │   ├── IndeedClone        # Main job search module
    │   ├── JobDashboard       # Recruiter dashboard
    │   ├── Shared             # Shared components used across modules
    │   └── SubModules
    │       ├── Auth           # Login, Register, OTP (2FA), Forgot Password, Google Sign-In
    │       ├── JobApplication # Job seeker module (CV upload, experience, screening questions)
    │       └── JobPost        # Employer job posting workflow
    │
    ├── Storage                # Stores uploaded user files (resumes)
    │
    └── ThirdParty             # Custom helper libraries
```

### Note on Modules (HMVC Architecture)

This project follows a modular HMVC architecture.  
Each folder inside the `Modules` directory is a self-contained module.

Every module typically includes its own:

- Controllers
- Models
- DTOs
- Enums
- Helpers
- ServiceContracts
- Services
- RepoContracts
- Repositories
- Views

This structure keeps modules independent and improves maintainability and scalability.
Some folders may contain some extra folder based on the pipeline workflow and behaviour.

## Tech Stack

- ASP.NET Core MVC
- C#
- SQL Server
- Entity Framework
- ADO.NET
- AJAX
- Razor Views
- Bootstrap

## Features

### Authentication
- User Login/Registration
- Forgot Password
- Email Verification Via OTP
- Google Sign-In

### Job Posting (Recruiter)
- Multi-step JobPost workflow (8 pages)
- Draft and Activate job system
- Transaction-based activation

### Job Search
- Keyword and Location search
- Time Filtering
- Location filtering
- Salary filtering
- Job type filtering
- Company Filtering
- Education Filtering
- Salary filtering
- Pagination

### Job Application
- Apply to jobs
- Resume upload
- Resume preview (PDF)
- Resume download
- Relevent Experience
- Employer Screener Questions

### Recruiter Dashboard
- Employer posted Jobs list
- Applicant list
- Status update (Shortlisted / Rejected)
- Live filtering
- Pagination

## Architecture

- Modular ASP.NET structure
- Solid Principles
- Repository Pattern
- Service Layer
- DTO pattern
- Centralized Error Handling (ErrorError Library)

## Author

Shubham Borude
+91 - 9370950037
shubhamborude4488@gmail.com
