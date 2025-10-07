## Part 1 – System Design (open brief)

> **Problem in one sentence:** > _“A user gives us some data & supporting documents, and we must return a finished, high-quality PDF.”_

### Your Task

Imagine you’re the first engineer on the project. Sketch a complete, end-to-end solution that turns **incoming user data** (structured fields _and_ uploaded files) into a **generated PDF** that blends that data with AI-generated prose.

_That’s it._
How you slice the problem is up to you—be opinionated, explore alternatives, and show us the trade-offs you’d make. I want to see how you think through an ambiguous business problem. Show me your ability to break down a problem.

### What to hand in

- A single Markdown (or PDF, your choice) document in a `/design` folder.
- Any diagrams or code snippets you feel strengthen your case (optional, not required).
- Length is flexible; depth is more important than page count.

### Questions we hope you’ll answer (interpret freely)

- **Architecture & Flow:** How does data enter, where does it live, and what are the major components?
- **AI & Retrieval:** Would you use AI? If you’d use embedding/RAG, how & why? If not, what’s better?
- **PDF Generation:** What tool(s) or template engines would you pick and why?
- **Scaling & Ops:** How would your design behave on launch day vs. 10× growth?
- **Security & Compliance:** Any red flags? How would you guard PII?
- **Trade-offs & Future Work:** Where are you punting for v1, and what would you improve later?

Treat those bullets as prompts, not a mandatory outline—feel free to reorder, merge, or ignore them if you have a sharper narrative.

### How we’ll review

| Dimension              | What impresses us                                                    |
| ---------------------- | -------------------------------------------------------------------- |
| **Clarity**            | We can follow your reasoning without jumping on a call.              |
| **Problem Solving**    | New angles, tool choices, or mental models.                          |
| **Trade-off thinking** | You identify risks and consciously defer or mitigate them.           |
| **Communication**      | Diagrams, analogies, or structure that make the complex feel simple. |

There’s no “right” answer—surprise us!
