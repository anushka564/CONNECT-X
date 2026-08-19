# Connect X

AI-Driven Career Intelligence and Opportunity Management Platform

ConnectX is a cloud-native, AI-driven career intelligence platform designed to connect students with relevant internships, jobs, placements, projects, and other career opportunities.

The platform addresses a common problem in student career discovery: opportunities are distributed across multiple channels such as college portals, emails, messaging platforms, social media, job portals, and company websites. Students must manually discover opportunities, understand eligibility criteria, compare requirements with their skills, track deadlines, and determine which opportunities are actually relevant to them.

ConnectX centralizes this process and uses Artificial Intelligence, semantic matching, document intelligence, cloud-native infrastructure, and personalized recommendations to help students discover and pursue opportunities more effectively.

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-20.x-green.svg)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue.svg)
![React](https://img.shields.io/badge/Frontend-React-61DAFB.svg)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-brightgreen.svg)
![AWS](https://img.shields.io/badge/Cloud-AWS-orange.svg)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow.svg)

## Table of Contents

- [Project Vision](#project-vision)
- [Problem Statement](#problem-statement)
- [Proposed Solution](#proposed-solution)
- [Core Objectives](#core-objectives)
- [Target Users](#target-users)
  - [Students](#students)
  - [Administrators](#administrators)
  - [Super Administrators](#super-administrators)
- [Major Features](#major-features)
  - [Authentication and Authorization](#authentication-and-authorization)
  - [Student Profile](#student-profile)
  - [Resume Intelligence](#resume-intelligence)
  - [Opportunity Management](#opportunity-management)
  - [Job Description Intelligence](#job-description-intelligence)
  - [Eligibility Engine](#eligibility-engine)
  - [AI Matching Engine](#ai-matching-engine)
  - [Matching Strategy](#matching-strategy)
  - [Explainable AI](#explainable-ai)
  - [Semantic Skill Matching](#semantic-skill-matching)
  - [Personalized Recommendation Engine](#personalized-recommendation-engine)
  - [Skill Gap Analysis](#skill-gap-analysis)
  - [AI Career Assistant](#ai-career-assistant)
  - [Retrieval-Augmented Generation](#retrieval-augmented-generation)
  - [Automated Opportunity Ingestion](#automated-opportunity-ingestion)
  - [Duplicate Opportunity Detection](#duplicate-opportunity-detection)
  - [Opportunity Classification](#opportunity-classification)
  - [Deadline Intelligence](#deadline-intelligence)
  - [Notifications](#notifications)
  - [Application Tracking](#application-tracking)
  - [Admin Dashboard](#admin-dashboard)
  - [Analytics](#analytics)
- [Technology Stack](#technology-stack)
- [High-Level Architecture](#high-level-architecture)
- [Cloud Architecture Principles](#cloud-architecture-principles)
- [Event-Driven Architecture](#event-driven-architecture)
- [Security Architecture](#security-architecture)
- [Data Privacy](#data-privacy)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
  - [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [API Overview](#api-overview)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)

## Project Vision

The vision of ConnectX is to build an intelligent career ecosystem rather than another conventional job portal.

Traditional platforms primarily answer: "What opportunities are available?"

ConnectX aims to answer: "Which opportunities are relevant to me, why are they relevant, what am I eligible for, what skills am I missing, and what should I do next?"

The core principle:

> ConnectX does not simply display opportunities. It understands the student, understands the opportunity, and intelligently connects the two.

## Problem Statement

Students often struggle to discover and evaluate relevant internships, jobs, and placement opportunities because information is fragmented across multiple communication channels and platforms.

Opportunities may be distributed through:

- College placement portals
- Email
- WhatsApp
- Telegram
- LinkedIn
- Company websites
- Job portals
- Faculty announcements
- Student communities
- PDFs
- Excel/CSV files
- Google Forms
- Other external sources

Students must manually determine:

1. Whether an opportunity is relevant.
2. Whether they satisfy the eligibility criteria.
3. Whether their skills match the job requirements.
4. Which skills they are missing.
5. When the application deadline is.
6. Where and how to apply.
7. Which opportunities should receive priority.
8. Which opportunities align with their career goals.

Existing job portals generally provide search, filtering, and keyword-based recommendations, but they do not necessarily provide a comprehensive understanding of a student's complete profile and the semantic relationship between the student's capabilities and the opportunity requirements.

This creates information overload, inefficient searching, missed opportunities, and poor personalization.

## Proposed Solution

ConnectX provides a centralized platform where students can maintain their career profiles and discover opportunities through an intelligent recommendation engine.

The platform combines:

- Student profile management
- Resume intelligence
- Opportunity management
- Job description intelligence
- Eligibility analysis
- Semantic skill matching
- Personalized recommendations
- Skill-gap analysis
- AI career assistance
- Opportunity classification
- Duplicate detection
- Deadline intelligence
- Application tracking
- Cloud-native processing
- Event-driven automation
- Security and auditability

## Core Objectives

| Objective | Description |
| --- | --- |
| Centralize Opportunities | Provide a single platform for discovering internships, jobs, placements, projects, competitions, certifications, and other career opportunities. |
| Personalize Discovery | Recommend opportunities based on skills, education, CGPA, graduation year, department, experience, career interests, preferred roles, preferred locations, and previous interactions. |
| Automate Opportunity Understanding | Automatically extract structured information from PDFs, documents, images, text, CSV files, Excel files, and job descriptions. |
| Improve Eligibility Verification | Use deterministic rules for hard eligibility requirements such as minimum CGPA, graduation year, department, degree, experience requirements, and location restrictions. |
| Provide Explainable Recommendations | Explain why an opportunity matches, the matching skills, missing skills, eligibility status, match score, and important requirements. |
| Identify Skill Gaps | Compare a student's current capabilities with target opportunity requirements and identify missing or weak skills. |
| Build a Scalable Cloud Platform | Use cloud-native infrastructure for scalable processing, secure document storage, asynchronous workloads, AI processing, monitoring, notifications, and automated deployments. |

## Target Users

| Role | Description |
| --- | --- |
| STUDENT | Discover opportunities, build a career profile, get recommendations, and track applications. |
| ADMIN | Create and manage opportunities, review AI-extracted information, and monitor platform activity. |
| SUPER_ADMIN | Manage administrators, system configuration, permissions, audit logs, and governance. |

### Students

Students can register and authenticate, build a career profile (education, skills, projects, certifications, experience, resume, preferences), upload resumes, define career interests and preferred roles or locations, discover opportunities with match scores, understand eligibility, identify skill gaps, save opportunities, track applications, receive notifications, and interact with the AI career assistant.

### Administrators

Administrators can create opportunities, upload opportunity documents, import CSV/Excel data, review and approve AI-extracted information, edit, publish or unpublish opportunities, manage students, categories and deadlines, monitor applications, review AI processing, and view analytics.

### Super Administrators

Super administrators can manage administrators and permissions, manage system configuration and platform-wide settings, review audit logs, manage AI policies and data governance, and monitor system health.

## Major Features

### Authentication and Authorization

Secure authentication with role-based authorization. Roles: STUDENT, ADMIN, SUPER_ADMIN.

Authorization is always enforced on the backend. Frontend role restrictions alone are not considered security controls.

### Student Profile

A student profile contains:

| Section | Contents |
| --- | --- |
| Personal Information | Name, contact, basic profile data |
| Academic Information | Degree, department, CGPA, graduation year |
| Skills | Skill names with proficiency levels |
| Projects | Titles, descriptions, technologies, links |
| Certifications | Names, issuers, validity |
| Experience | Roles, companies, durations |
| Resume | Stored document and extracted data |
| Preferences | Preferred roles, locations, career interests, target technologies |
| Application History | Applied, saved, and tracked opportunities |

```
Student
├── Education
├── Skills
├── Projects
├── Certifications
├── Experience
├── Resume
├── Preferences
└── Applications
```

### Resume Intelligence

Students can upload resumes in supported formats. The processing pipeline:

```
Resume Upload
     |
     v
Private Cloud Storage
     |
     v
Document Processing
     |
     v
Text Extraction
     |
     v
AI/NLP Processing
     |
     v
Structured Student Profile
     |
     v
Validation
     |
     v
Profile Update
```

The system may extract name, education, skills, projects, certifications, experience, technologies, domains, and achievements.

AI-generated information is treated as extracted information and never silently overwrites user-provided information without validation.

### Opportunity Management

Each opportunity contains structured information:

| Field | Description |
| --- | --- |
| Company | Organization offering the opportunity |
| Title | Role or position title |
| Description | Full description text |
| Category | Classification such as Cloud Computing or Cybersecurity |
| Required Skills | Skills required for the role |
| Eligibility | Eligibility criteria text |
| Minimum CGPA | Deterministic CGPA cutoff |
| Graduation Year | Eligible graduation batches |
| Eligible Departments | Departments allowed to apply |
| Experience | Required experience level |
| Location | Work location |
| Work Mode | On-site, remote, or hybrid |
| Salary/Stipend | Compensation details |
| Deadline | Application deadline |
| Application URL | Where to apply |
| Source | Origin of the opportunity |
| Status | Lifecycle status (table below) |
| Verification Status | AI-extracted or admin-verified |
| Created/Updated Timestamp | Audit timestamps |

| Status | Meaning |
| --- | --- |
| DRAFT | Created but not submitted for review |
| PENDING_REVIEW | Awaiting admin verification |
| PUBLISHED | Visible to students |
| EXPIRED | Deadline passed |
| ARCHIVED | Retired from active listing |
| REJECTED | Rejected during review |

### Job Description Intelligence

When a job description is uploaded, ConnectX extracts role, company, skills, eligibility, experience, education, location, salary/stipend, deadline, responsibilities, preferred skills, and application URL.

```
Job Description
     |
     v
Document Extraction
     |
     v
Text Normalization
     |
     v
AI Extraction
     |
     v
Structured Opportunity
     |
     v
Validation
     |
     v
Admin Review
     |
     v
Publication
```

AI must not automatically publish unverified information.

### Eligibility Engine

Eligibility primarily uses deterministic rules for hard constraints. Example:

```
CGPA >= 7.0
AND
Graduation Year = 2027
AND
Department IN [CSE, ISE, CTIS]
```

Result: ELIGIBLE or NOT_ELIGIBLE.

AI may explain the result but should not replace deterministic eligibility logic for hard constraints.

### AI Matching Engine

The matching engine compares the student profile with opportunity requirements:

```
Student Profile
        +
Opportunity Requirements
        |
        v
Matching Engine
        |
        v
Match Score
        +
Matched Skills
        +
Missing Skills
        +
Eligibility
        +
Explanation
```

Example output:

```
Match Score: 88%

Matched Skills:
- AWS
- Python
- Linux
- Networking

Missing Skills:
- IAM
- Terraform

Eligibility: Eligible
Recommendation: Strong Match
```

### Matching Strategy

ConnectX does not rely exclusively on keyword matching. The recommended approach is a hybrid architecture:

```
Hard Eligibility Rules
          +
Skill Normalization
          +
Semantic Embeddings
          +
Weighted Ranking
          +
User Preferences
          |
          v
Final Recommendation Score
```

Example scoring model. Weights are configurable and the exact formula must be validated through testing and real usage data rather than assumed to be optimal.

| Component | Weight |
| --- | --- |
| Skill Match | 40% |
| Eligibility | 20% |
| Experience Match | 15% |
| Role Preference | 10% |
| Location Preference | 10% |
| Deadline/Urgency | 5% |

### Explainable AI

Every recommendation includes an explanation. The platform avoids opaque recommendations whenever possible.

```
88% Match

Why:
- Strong AWS experience
- Strong Python experience
- Strong Linux knowledge
- Relevant cybersecurity projects
- Eligible graduation year

Skill Gaps:
- AWS IAM
- Terraform

Recommendation:
Consider learning IAM and Terraform to improve suitability.
```

### Semantic Skill Matching

Different representations of the same concept are normalized:

| Variant | Normalized |
| --- | --- |
| Amazon Web Services | AWS |
| Amazon EC2 | EC2 |
| JavaScript | JS |
| Artificial Intelligence | AI |
| Machine Learning | ML |

Semantic embeddings are used to identify related concepts, moving beyond exact keyword matching.

### Personalized Recommendation Engine

Opportunities are ranked using student skills, academic profile, career goals, preferred roles, preferred locations, experience, eligibility, previous applications, saved opportunities, and interaction history. Students see a personalized feed:

```
Recommended for You

Cloud Security Intern       94%
SOC Analyst Intern          89%
AWS Cloud Intern            86%
DevOps Intern               83%
```

### Skill Gap Analysis

The difference between current student skills and target opportunity requirements:

```
Current Student Skills
        |
        v
Target Opportunity Requirements
        |
        v
Skill Gap
```

Example:

```
Current Skills:  AWS, Linux, Python, Networking
Required:        AWS, Linux, Python, Networking, IAM, Terraform, SIEM
Skill Gap:       IAM, Terraform, SIEM
```

The platform can then recommend learning resources or projects to close the gap.

### AI Career Assistant

A conversational AI assistant answers questions such as:

- Which cloud internships am I eligible for?
- What skills am I missing for this job?
- Which opportunity should I apply for first?
- What should I learn to become a cloud security engineer?
- Why was this opportunity recommended to me?
- Show me opportunities closing this week.

The assistant retrieves verified ConnectX data before answering questions related to current opportunities.

### Retrieval-Augmented Generation

For domain-specific questions, ConnectX uses RAG:

```
User Question
     |
     v
Intent Detection
     |
     v
Retrieval
     |
     v
ConnectX Knowledge Base
     |
     v
Relevant Documents/Data
     |
     v
LLM
     |
     v
Grounded Response
```

Potential knowledge sources include opportunity descriptions, placement policies, career guides, skill definitions, learning resources, and verified university information. The system distinguishes between verified platform data and general AI-generated guidance.

### Automated Opportunity Ingestion

ConnectX supports multiple input sources:

| Source | Example |
| --- | --- |
| PDF | Job description attachments |
| Excel | Bulk opportunity sheets |
| CSV | Imported placement data |
| Text | Pasted job descriptions |
| Image | Flyers and screenshots |
| Admin Form | Manual entry |
| API | External system integration |

```
Source
  |
  v
Document Processing
  |
  v
Information Extraction
  |
  v
Normalization
  |
  v
Duplicate Detection
  |
  v
Validation
  |
  v
Admin Approval
  |
  v
Publication
```

Human approval remains available for sensitive or uncertain records.

### Duplicate Opportunity Detection

Potential duplicates are identified by comparing company, role, description, deadline, application URL, required skills, and location.

```
Potential Duplicate: 93%

Existing:
Cloud Security Intern - XYZ

New:
Cloud Security Internship - XYZ Technologies
```

The administrator confirms whether the records should be merged.

### Opportunity Classification

AI can automatically classify opportunities. Administrators can modify classifications.

| Category |
| --- |
| Software Development |
| Cloud Computing |
| Cybersecurity |
| Cloud Security |
| DevOps |
| Data Science |
| Artificial Intelligence |
| Machine Learning |
| Networking |
| Finance |
| Marketing |
| Design |
| Research |
| Other |

### Deadline Intelligence

Deadlines are normalized into machine-readable timestamps. The system can identify: closing today, closing tomorrow, closing in 3 days, closing this week, or expired. The configured timezone is used and ambiguous date interpretation is avoided.

### Notifications

| Notification | Trigger |
| --- | --- |
| New highly relevant opportunity | High match score on a new opportunity |
| Application deadline approaching | Deadline within a configured window |
| Application status update | Status change on a tracked application |
| Saved opportunity closing soon | Deadline of a saved opportunity approaching |
| Profile incomplete | Missing required profile fields |
| Skill-gap recommendation | Gap identified between profile and target role |
| Admin announcement | Broadcast from administrators |

Notification channels can later include in-app, email, and push. Preferences are user-configurable.

### Application Tracking

| State | Meaning |
| --- | --- |
| SAVED | Saved for later |
| APPLIED | Application submitted |
| ASSESSMENT | Under screening or assessment |
| INTERVIEW | Interview stage |
| SHORTLISTED | Shortlisted by the recruiter |
| SELECTED | Offer received |
| REJECTED | Not selected |
| WITHDRAWN | Withdrawn by the student |

Example:

```
Cloud Security Intern
Status: Interview
Applied: 15 Aug 2026
Next Step: Technical Interview
```

### Admin Dashboard

Provides a single view of total students, active opportunities, applications, upcoming deadlines, expired opportunities, pending reviews, AI processing status, potential duplicates, and system health. Administrators manage the entire opportunity lifecycle from this dashboard.

### Analytics

Potential analytics include:

- Most popular roles
- Most requested skills
- Most active companies
- Application conversion rate
- Opportunity category distribution
- Student skill distribution
- Most common skill gaps
- Department-wise applications
- Opportunity engagement
- Application deadlines

AI can later identify trends (for example, "AWS and cybersecurity skills are increasingly requested"). Such insights must be based on actual platform data.

## Technology Stack

| Layer | Technology |
| --- | --- |
| Frontend | React, TypeScript, Vite, Tailwind CSS, React Query |
| Backend | Node.js, Express.js, TypeScript, REST APIs |
| Database (initial) | MongoDB |
| Database (production candidate) | Amazon Aurora PostgreSQL |
| Storage | Amazon S3 |
| Authentication | Amazon Cognito (or approved identity provider) |
| AI | Amazon Bedrock |
| Document Processing | Amazon Textract |
| Vector Search | Amazon OpenSearch Serverless (or managed vector database) |
| Cloud Compute | AWS Lambda, Amazon ECS Fargate |
| Messaging | Amazon SQS, Amazon EventBridge |
| Notifications | Amazon SES, Amazon SNS |
| Monitoring | Amazon CloudWatch |
| Secrets | AWS Secrets Manager |
| Containers | Docker |
| CI/CD | GitHub Actions, Amazon ECR |
| Infrastructure as Code | Terraform |

## High-Level Architecture

```
                         CONNECTX
                            |
             +--------------+--------------+
             |                             |
       Student Portal                Admin Portal
             |                             |
             +--------------+--------------+
                            |
                     API Gateway / ALB
                            |
                    Backend Services
                            |
          +-----------------+-----------------+
          |                 |                 |
      User Service    Opportunity Service   Application
          |                 |                 |
          +-----------------+-----------------+
                            |
                      Event-Driven Layer
                            |
             +--------------+--------------+
             |                             |
        Amazon EventBridge             Amazon SQS
             |                             |
          Lambda                        Workers
             |                             |
             +--------------+--------------+
                            |
                       AI Processing
                            |
          +-----------------+-----------------+
          |                 |                 |
       Textract          Bedrock        Embeddings
          |                 |                 |
          +-----------------+-----------------+
                            |
                     Knowledge Layer
                            |
              +-------------+-------------+
              |                           |
          Primary DB                 Vector Store
              |                           |
              +-------------+-------------+
                            |
                         Amazon S3
```

## Cloud Architecture Principles

| Principle | Application |
| --- | --- |
| Scalability | Services scale independently where appropriate. |
| Reliability | Asynchronous workloads use queues and retry mechanisms. |
| Security | Least-privilege IAM and private resources. |
| Observability | Log important application and infrastructure events. |
| Cost Optimization | Avoid unnecessarily expensive always-on infrastructure. |
| Fault Tolerance | Failures in AI processing do not bring down the core application. |
| Automation | Use CI/CD and infrastructure-as-code where practical. |

## Event-Driven Architecture

Expensive AI processing never blocks normal API requests. Example resume-processing workflow:

```
Student Uploads Resume
        |
        v
Amazon S3
        |
        v
ResumeUploaded Event
        |
        v
EventBridge
        |
        v
SQS
        |
        v
Processing Worker
        |
        +----> Textract
        |
        +----> Bedrock
        |
        +----> Embedding Generation
        |
        v
Profile Updated
        |
        v
Matching Engine
        |
        v
Recommendations Updated
```

This prevents expensive AI processing from blocking normal API requests.

## Security Architecture

ConnectX may process sensitive student information. Security controls include:

### Authentication

- Secure authentication
- MFA where appropriate
- Session management
- Token validation

### Authorization

- Role-based access control
- Backend-enforced authorization
- Resource-level authorization

### Data Protection

- TLS in transit
- Encryption at rest
- Private S3 buckets
- Database encryption
- Secure backups

### Secrets Management

Never commit API keys, passwords, JWT secrets, AWS credentials, or database credentials. Use AWS Secrets Manager, environment variables, and GitHub Actions Secrets as appropriate.

## Data Privacy

ConnectX follows privacy-by-design principles:

- Collect only the information necessary to provide career matching and recommendation services.
- Clearly communicate why information is collected, how it will be used, and how long it will be retained, at the point of collection and in the privacy policy.
- Allow students to access, correct, export, and delete their personal data.
- Obtain explicit consent before AI processing of uploaded documents, and clearly label AI-extracted fields for validation.
- Apply purpose limitation: student data is used only for the intended career services and is never sold or shared with third parties without consent.
- Enforce role-based access so personal data is visible only to the student and to authorized administrators.
- Retain data only for as long as needed, and delete or anonymize it after account closure or at the end of the retention period.
- Comply with applicable data protection regulations (for example, GDPR, the DPDP Act, or other regional requirements).

## Getting Started

### Prerequisites

- Node.js 20 or later
- npm or yarn
- MongoDB (local instance or MongoDB Atlas)
- AWS account (for Bedrock, Textract, S3, Cognito, SQS, EventBridge)
- Docker (for local containers)
- Terraform (for infrastructure provisioning)

### Installation

1. Clone the repository and install dependencies:

```bash
git clone https://github.com/<your-org>/connectx.git
cd connectx
```

2. Install backend dependencies:

```bash
cd server
npm install
```

3. Install frontend dependencies:

```bash
cd ../client
npm install
```

4. Configure environment variables (see below).

5. Run database migrations and seed data if applicable.

### Environment Variables

| Variable | Description | Example |
| --- | --- | --- |
| PORT | API server port | 4000 |
| NODE_ENV | Runtime environment | development |
| MONGODB_URI | MongoDB connection string | mongodb://localhost:27017/connectx |
| JWT_SECRET | Secret used to sign access tokens | change-me |
| AWS_REGION | AWS region for all AWS services | us-east-1 |
| S3_BUCKET | Private S3 bucket for resumes and documents | connectx-private-assets |
| COGNITO_USER_POOL_ID | Cognito user pool identifier | us-east-1_xxxxx |
| COGNITO_CLIENT_ID | Cognito app client identifier | xxxxx |
| BEDROCK_MODEL_ID | Bedrock model for extraction and matching | anthropic.claude-3-5-sonnet-20241022 |
| VECTOR_INDEX | OpenSearch Serverless vector index name | skill-embeddings |
| SES_FROM_EMAIL | Verified sender address for notifications | no-reply@connectx.dev |
| TIMEZONE | Platform timezone used for deadline logic | Asia/Kolkata |

Copy `server/.env.example` to `server/.env` and fill in the values. Never commit `.env` files.

### Running the Application

```bash
# Backend API
cd server
npm run dev

# Frontend app
cd client
npm run dev
```

The frontend runs on http://localhost:5173 and the API on http://localhost:4000 by default.

## Project Structure

```
connectx/
├── client/                    # React frontend (Vite + TypeScript + Tailwind)
│   ├── src/
│   │   ├── components/        # Reusable UI components
│   │   ├── pages/             # Route-level pages
│   │   ├── hooks/             # Custom React hooks
│   │   ├── services/          # API client and query layer
│   │   └── types/             # Shared TypeScript types
│   └── package.json
├── server/                    # Node.js/Express backend (TypeScript)
│   ├── src/
│   │   ├── api/               # REST route handlers
│   │   ├── services/          # Business logic
│   │   ├── models/            # Data models
│   │   ├── middleware/        # Auth, validation, error handling
│   │   ├── ai/                # Bedrock, Textract, embedding integrations
│   │   ├── workers/           # Async queue consumers
│   │   └── config/            # Environment and app configuration
│   ├── tests/                 # Unit and integration tests
│   └── package.json
├── infra/                     # Terraform infrastructure as code
├── .github/workflows/         # CI/CD pipelines
├── .env.example
├── docker-compose.yml
└── README.md
```

## API Overview

All protected endpoints require a Bearer token. Authorization is always enforced server-side.

| Method | Endpoint | Access | Description |
| --- | --- | --- | --- |
| POST | /api/auth/register | Public | Register a student account |
| POST | /api/auth/login | Public | Authenticate and obtain a token |
| GET | /api/students/me | STUDENT | Get the current student profile |
| PUT | /api/students/me | STUDENT | Update the student profile |
| POST | /api/students/me/resume | STUDENT | Upload a resume for processing |
| GET | /api/opportunities | STUDENT, ADMIN | List opportunities (ranked for students) |
| GET | /api/opportunities/:id | STUDENT, ADMIN | Opportunity details with match explanation |
| POST | /api/opportunities | ADMIN | Create an opportunity |
| PUT | /api/opportunities/:id | ADMIN | Update an opportunity |
| POST | /api/opportunities/import | ADMIN | Import opportunities from PDF/CSV/Excel |
| POST | /api/opportunities/:id/approve | ADMIN | Approve and publish an opportunity |
| GET | /api/recommendations | STUDENT | Personalized opportunity feed |
| POST | /api/opportunities/:id/save | STUDENT | Save an opportunity |
| GET | /api/applications | STUDENT, ADMIN | List applications |
| POST | /api/applications | STUDENT | Submit an application |
| PATCH | /api/applications/:id/status | ADMIN | Update application status |
| POST | /api/assistant/chat | STUDENT | Ask the AI career assistant |
| GET | /api/admin/analytics | ADMIN | Analytics dashboard data |
| GET | /api/admin/audit-logs | SUPER_ADMIN | Audit log review |

## Roadmap

| Phase | Scope |
| --- | --- |
| Phase 1 - Foundation | Authentication and RBAC, student profiles, opportunity CRUD, admin portal, application tracking |
| Phase 2 - Intelligence | Resume parsing, JD extraction, eligibility engine, hybrid matching engine, explainable recommendations |
| Phase 3 - Scale | RAG career assistant, automated ingestion pipelines, duplicate detection, notifications, analytics |
| Phase 4 - Productionization | Terraform infrastructure, CI/CD, monitoring and alerting, load and penetration testing, tenant hardening |

## Contributing

Contributions are welcome. Please follow the standard flow:

1. Fork the repository.
2. Create a feature branch.
3. Make your changes with tests.
4. Open a pull request describing the change and any related issue.

Follow the existing code style, keep TypeScript strict mode enabled, and never commit secrets.

## License

MIT License. See the LICENSE file for details.
