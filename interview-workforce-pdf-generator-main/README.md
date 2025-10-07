# Workforce Visas - Technical Interview

Welcome to the Workforce Visas technical interview! This is a comprehensive assessment designed to evaluate your technical skills, problem-solving abilities, and system design thinking.

## Interview Overview

This interview consists of **two parts** and we are paying for **two hours of your time** to complete both components:

1. **System Design Challenge**
2. **Coding Challenge**

## Part 1: System Design Challenge - details in the **system-design.md**

### Overview

You'll be working on an open-ended system design problem where you need to sketch a complete, end-to-end solution that turns **incoming user data** (structured fields and uploaded files) into a **generated PDF** that blends that data with AI-generated prose.

### What You'll Do

- Design a complete system architecture
- Consider AI integration and retrieval strategies
- Plan PDF generation approaches
- Think about scaling, security, and compliance
- Document your design decisions and trade-offs

### Deliverable

- A single Markdown document in the `/system-design` folder
- Optional diagrams or code snippets
- Focus on depth over length

## Part 2: Coding Challenge - "From Form to PDF" - details in the **coding-challenge.md**

### Overview

You'll build a tiny Next.js feature that takes **user-submitted data + an uploaded file** and turns it into a **single PDF**.

### User Flow

1. **Entry point** – User visits `/apply`
2. **Form** – They fill out basic personal details and specify their current job description
3. **Upload** – They attach one supporting document (PDF file type)
4. **Submit** – After form submission:
   - Persist everything in the repo (FS, JSON - your choice)
   - Generate a PDF containing:
     - User's personal details (nicely formatted header)
     - Job description paragraph
     - Content from the uploaded file (or a note that it's stored)
   - Return a download link or modal for the PDF

### Technical Requirements

- **Database:** SQLite with Prisma (self-contained, no hosted DB needed)
- **File Storage:** Local file system (`./uploads` folder)
- **PDF Generation:** Your choice of library (`pdf-lib`, `@react-pdf/renderer`, etc.)
- **Styling:** Minimal UI - focus on backend logic and code

### Deliverables

1. **Running code** committed to your repo
2. **`/coding-challenge` folder** with:
   - Data model explanation (ER diagram, schema file, or bullet list)
   - Request flow documentation

## What We're Looking For

| Area               | What to Demonstrate                                         |
| ------------------ | ----------------------------------------------------------- |
| **Data Modeling**  | Clear representation of how data model relate               |
| **Code Structure** | Separation of concerns, clear naming, testability           |
| **PDF Generation** | Smart library choice and working implementation             |
| **System Design**  | Thoughtful architecture decisions and trade-off analysis    |
| **Edge Cases**     | Basic validation, error handling, graceful failure handling |
| **Documentation**  | Clear README and design documentation                       |

## Ground Rules

- **File Storage:** Use local file system (`./uploads` folder)
- **Styling:** Keep UI minimal - focus on backend logic
- **Libraries:** Use any publicly available npm packages
- **Secrets:** Don't commit API keys - add needed env var constants to `.env.example`

## Submission Process

1. Fork this repo to your GitHub account
2. Complete both parts of the interview
3. Open a Pull Request **to this repo's `main` branch**
4. In the PR description, include your name and any additional context

## Getting Started

1. Read through both challenge documents thoroughly
2. Set up your development environment
3. Start with whichever part feels most comfortable to you
4. Document your decisions and reasoning as you go

Good luck! We're excited to see your approach and solutions.
