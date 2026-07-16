# gen-ai-interview — AI Interview Strategy Generator

## Tech Stack
- Frontend: **React (Hooks), React Router, SCSS**
- Backend: **Node.js, Express, Multer (file upload)**
- AI/LLM: **Google Gemini (GoogleGenAI), Zod (schema validation), Zod-to-JSON-Schema**
- PDF Generation: **Puppeteer (HTML → PDF)**
- Auth: **JWT middleware (authUser)**

## Resume Bullets (Scalable / Number Data)
- Built an AI-powered interview planner that converts a user’s **resume (PDF/DOCX text extraction)** + **job description** into a structured plan including **matchScore (0–100), technical/behavioral questions, skill gaps (low/medium/high), and a day-wise preparation roadmap**.
- Implemented **LLM structured-output** using **Zod schemas** to enforce valid JSON responses (reducing malformed outputs) and drive deterministic UI rendering across multiple interview sessions.
- Delivered **ATS-friendly resume PDF generation** by producing job-tailored **HTML** via Gemini and rendering it with **Puppeteer**, enabling one-click downloads for interview-ready resumes.
- Designed secure, user-scoped endpoints (**create report / fetch by id / list user reports / generate resume PDF**) with **auth middleware + multipart uploads** to support scalable usage across multiple candidates.
- Optimized end-to-end workflow so users get results in **~30 seconds** (conservative estimate shown in UI) and can manage **multiple generated interview plans per account** (scalable to large backlogs via persisted reports).

