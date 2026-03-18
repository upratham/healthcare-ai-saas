# MediNotes AI

An AI-powered healthcare SaaS application that helps doctors convert consultation notes into structured medical summaries, next steps, and patient-friendly email drafts. Built as a full-stack app with secure authentication, subscription-based access, and real-time AI streaming on Vercel. :contentReference[oaicite:0]{index=0}

## Features

- Secure user authentication with Clerk
- Subscription-based access control with Clerk Billing
- AI-generated consultation summaries
- Doctor action items from visit notes
- Patient-friendly email drafting
- Real-time streaming responses
- Clean and responsive UI
- Serverless deployment on Vercel

## Tech Stack

Next.js, React, TypeScript, Tailwind CSS, FastAPI, Pydantic, OpenAI API, Clerk Authentication, Clerk Billing, Vercel :contentReference[oaicite:1]{index=1} :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

## Project Overview

MediNotes AI is designed for healthcare professionals who want to reduce time spent on manual documentation. The application accepts consultation details such as patient name, date of visit, and doctor notes, then generates three structured outputs:

- Summary of visit for medical records
- Next steps for the doctor
- Draft email to the patient in patient-friendly language

This healthcare workflow is described in the project transformation steps from the uploaded notes. :contentReference[oaicite:4]{index=4} :contentReference[oaicite:5]{index=5}

## How It Works

1. Users sign in securely using Clerk
2. Access to the product is protected by subscription checks
3. Doctors enter consultation details into the form
4. The frontend sends authenticated requests to the FastAPI backend
5. The backend verifies JWT tokens using Clerk
6. OpenAI generates structured healthcare output
7. Results are streamed back to the UI in real time

This architecture follows the app flow defined across the SaaS, Clerk auth, billing, and healthcare setup files. :contentReference[oaicite:6]{index=6} :contentReference[oaicite:7]{index=7} :contentReference[oaicite:8]{index=8} :contentReference[oaicite:9]{index=9}

## Folder Structure

```bash
.
├── pages/              # Next.js frontend pages
├── api/                # FastAPI backend
├── styles/             # Global styles
├── public/             # Static assets
├── requirements.txt    # Python dependencies
├── package.json        # Frontend dependencies
└── .env.local          # Environment variables
