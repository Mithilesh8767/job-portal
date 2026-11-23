# Job Portal

A full-stack web application designed to connect job seekers with recruiters through a centralized online recruitment platform. Job seekers can discover opportunities, manage their profiles, upload resumes, and apply for jobs. Recruiters can create company profiles, publish job openings, and review applications.

## Project Overview

The project focuses on making recruitment more organized and accessible by bringing job listings, candidate information, and applications into one platform.

The application supports two primary user roles:

- **Job Seeker (Student):** Explore job openings, maintain a profile, upload a resume, apply for suitable positions, and track application progress.
- **Recruiter:** Create and manage a company profile, publish and maintain job listings, and view and manage applications received for jobs.

## Key Features

### Job Seekers
- User registration and login.
- Create and update a user profile.
- Add skills and profile information.
- Upload a resume and profile photo.
- Browse and search available jobs.
- Filter job opportunities using criteria such as keywords, job type, and location.
- Apply for job openings.
- Track application status.

### Recruiters
- Recruiter registration and login.
- Create and manage a company profile.
- Post job openings with details such as title, description, required skills, salary, experience level, job type, and location.
- Update or remove job postings.
- View applicants for posted jobs.
- Manage candidate applications, including shortlisting or rejection.

### Platform
- Role-based access for job seekers and recruiters.
- Centralized storage for users, companies, jobs, and applications.
- Resume and image storage using Cloudinary.
- Responsive interface intended for desktop, tablet, and mobile use.

## Technology Stack

| Area | Technologies | Purpose |
|---|---|---|
| Frontend | React.js | Component-based user interface |
| Styling | Tailwind CSS | Responsive interface styling |
| Frontend routing | React Router | Navigation between application pages |
| HTTP requests | Axios | Communication with backend APIs |
| Backend | Node.js, Express.js | Server-side logic and REST API handling |
| Database | MongoDB | Storing users, companies, jobs, and applications |
| ODM | Mongoose | MongoDB schemas and data operations |
| Authentication | JSON Web Tokens (JWT) | User authentication and protected access |
| File storage | Cloudinary | Profile images and resume files |

## Application Workflow

1. A user registers and signs in as a job seeker or recruiter.
2. A job seeker completes their profile and can upload a resume.
3. A recruiter creates a company profile and publishes job openings.
4. Job seekers browse or filter available jobs and submit applications.
5. Recruiters review applications associated with their job postings and update candidate status.
6. Job seekers can check the status of their submitted applications.

## Data Model

The project report describes the main data entities as:

- **User:** Name, email, phone number, password, role, profile information, skills, resume details, profile photo, and company reference where applicable.
- **Company:** Company name, description, website, location, logo, and associated user.
- **Job:** Job title, description, requirements, salary, experience level, location, job type, company, and creator.
- **Application:** The related job, applicant, and application status (such as pending, accepted, or rejected).

## Getting Started

The project report identifies the MERN stack but does not specify the exact repository folder layout or all package scripts. Use the instructions below as a general setup guide and adjust the commands to match the `package.json` files in your repository.

### Prerequisites

- Node.js and npm
- MongoDB database (local or hosted)
- Cloudinary account for file uploads
- Git

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Install dependencies in the frontend and backend directories (where applicable):

   ```bash
   cd <frontend-folder>
   npm install
   ```

   ```bash
   cd <backend-folder>
   npm install
   ```

3. Create the environment file(s) required by the frontend and backend. Add the MongoDB connection string, JWT secret, Cloudinary credentials, and any frontend API base URL required by your implementation. Use the variable names expected by your source code; do not commit real credentials.

4. Start the backend and frontend using the scripts defined in their respective `package.json` files. For example, a project may use:

   ```bash
   npm run dev
   ```

   or:

   ```bash
   npm start
   ```

5. Open the local frontend URL printed in the terminal.

## Security Notes

- Keep `.env` files and all API keys, database credentials, and JWT secrets out of version control.
- Add environment files to `.gitignore`.
- Do not store plaintext passwords; use secure password hashing in the authentication implementation.
- Validate and authorize requests on the server, especially recruiter-only job-management actions and access to applicant information.

## Future Enhancements

The project report identifies the following possible extensions:

- AI-based job recommendations.
- Real-time chat or messaging between recruiters and candidates.
- Two-factor authentication and OAuth login (for example, Google or LinkedIn).
- Advanced analytics and recruitment dashboards.
- Video interview functionality.
- Mobile application support.
- Internship and freelance job categories.
- Skill-assessment tests.

## Contributors

- Mithilesh Anil Chousalkar
- Rushikesh Satyanaryan Takey
- Raghavendra Atulrao Anandgaonkar

