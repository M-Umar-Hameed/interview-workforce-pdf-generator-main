# Coding Challenge – “From Form to PDF”

Welcome!  
You’ll build a tiny Next.js feature that takes **user-submitted data + an uploaded file** and turns it into a **single PDF**.  
Most details are intentionally vague so you can show us how you think, structure data, and make trade-offs.

---

## 1 . The (deliberately loose) user flow

1. **Entry point** – A user visits `/apply`.
2. **Form** – They fill out basic personal details _and_ specify their **current job description** (plain text).
3. **Upload** – They attach **one supporting document** (pdf file type).
4. **Submit** – After the form posts:
   - Persist everything somewhere in the repo (FS, JSON - your choice, but no need to integrate a blob storage).
   - Generate a **PDF** that contains:
     - The user’s personal details (as a nicely formatted header).
     - The job-description paragraph they typed.
     - _Any_ content you choose from the uploaded file (or a note that it’s been stored).
   - Return a link or modal so the user can download that PDF.

That’s all! How you design the data model and plumbing is up to you.

---

## 2.a. Starter repo

We give you a minimal **Next.js 14 / TypeScript** skeleton:

Feel free to reorganize folders, add libs, or install packages.

## 2.b. 💾 Database Instructions

To keep this project self-contained, we’ll use **SQLite** with Prisma.

No hosted database is needed. Just follow these steps:

### 1. Set up

```bash
cp .env.example .env
npx prisma db push
```

---

## 3 . What we care about

| Area                   | What to demonstrate                                                                                                                     |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| **Data modeling**      | Show your reasoning: TS interfaces, Prisma schema, SQL DDL—any clear representation of how “User”, “Submission”, and “Document” relate. |
| **Code structure**     | Separation of concerns, clear naming, testability.                                                                                      |
| **PDF generation**     | Library choice is yours (`pdf-lib`, `@react-pdf/renderer`, LaTeX + puppeteer, etc.). The result just needs to open.                     |
| **DX & README**        | `pnpm install && pnpm dev` should run; explain any env vars or scripts.                                                                 |
| **Edge-case thinking** | Basic validation, error feedback, graceful failure on large files.                                                                      |

---

## 4 . Deliverables

1. **Running code** committed to your repo.
2. **`/design` folder** with a short Markdown note explaining:
   - Your data model (ER diagram, schema file, or bullet list).
   - How the request travels through your code.
3. (Optional) Unit or integration tests showing something you deem critical.

---

## 5 . Ground rules & hints

| Topic            | Guideline                                                                      |
| ---------------- | ------------------------------------------------------------------------------ |
| **File storage** | Skip S3/GCS; writing to `./uploads` (git-ignored) is fine.                     |
| **Styling**      | Keep UI minimal—focus is backend logic.                                        |
| **Libraries**    | Use anything publicly available via npm.                                       |
| **Secrets**      | Don’t commit API keys. If you need an env var, add an entry to `.env.example`. |
| **Time box**     | It’s okay to annotate unfinished areas with TODOs.                             |

---

## 6 . How to submit - Fork & Pull Request

1. Fork this repo to your own GitHub account (public is fine).
2. Complete the project in your fork.
3. Open a Pull Request **to this repo’s `main` branch**.
4. In the PR description, include your name and anything you want us to know.

Looking forward to seeing your approach—have fun and surprise us!
