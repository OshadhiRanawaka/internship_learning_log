# Internship Learning Week — Progress Log

## Overview
As part of the Learning Week during my Fullstack Developer Internship at ProLab R, I worked through a full-length course on building a production-ready job application tracker using Next.js, React, Tailwind CSS, and MongoDB. This README documents my daily progress and key takeaways.

## Resource
- **Video:** [NextJS 16 Full Course 2026 — Build and Deploy A Production Ready Job Application Tracker w/ MongoDB](https://youtu.be/vCIsrOGNhas)
- **Format:** Full-length, project-based tutorial
- **Tech Stack Covered:** Next.js 16, React, Tailwind CSS, ShadCN, MongoDB, Mongoose, Better Auth

## Daily Progress Log

**Day 1**
- Got an overview of the project: a full-stack job application tracker built with Next.js, React, Tailwind CSS, and MongoDB
- Set up the Next.js project and went over the front-end/back-end folder structure
- Introduced Tailwind CSS as a utility-first styling approach
- Set up ShadCN to add reusable, pre-built UI components without a full component library
- Learned Next.js's file-based routing system (folder names map directly to URL paths)
- Covered the difference between server and client components — server components for performance, client components for interactivity — and when to use each

**Day 2**
- Explored MongoDB as a flexible, schema-less database and how it compares to SQL tables (collections/documents, BSON format)
- Learned Mongoose as an ORM for working with MongoDB in a TypeScript environment
- Set up authentication using Better Auth
- Built the sign-up form: structuring inputs, managing loading/error state, and linking to the sign-in page
- Created API routes to handle sign-up and login requests
- Implemented session management and a user dropdown menu with a sign-out helper function

**Day 3**
- Designed the database schema for the job tracker: boards containing columns (e.g. Wish List, Applied, Interviewing), each holding multiple job applications, with indexed user IDs for faster queries
- Built the logic to automatically initialize a user's board with default columns when their account is created (checking for an existing board first to avoid duplicates)
- Added middleware (proxy.ts file) to check authentication status and redirect users appropriately between the dashboard and sign-in/sign-up pages
- Built the droppable Kanban-style column component, defining props/types (column, config, board ID) and dynamic color styling
- Built the "add job application" form using a Tailwind grid layout, with input fields (e.g. salary, job URL) which is managed by React state
- Implemented the create-job-application logic, which includes ownership verification for the board/column and default handling for optional fields like tags
- Built the job card component to render each application's details

**Day 4**
- Implemented caching in Next.js via `next.config.ts` and used Suspense components to handle loading states smoothly
- Used seed files to populate the database with mock job application data for testing
- Built a custom hook to manage job board state,  for the drag-and-drop
- Implemented server actions to update and deleteing job applications' columns and order, including logic for reordering within and across columns
- Completed full drag-and-drop functionality using a sortable contect along with drop validation, filtering out duplicates and a drag overlay for smoother UX
- 



## Key Takeaways
- Clear idea for when to use server vs. client components in Next.js, and why defaulting to server components improves performance
- Practical experience structuring a MongoDB schema
- Implementation of authentication end-to-end using Better Auth (sign-up, sign-in, sessions, sign-out)
- Exposure to Next.js caching (`next.config.ts`, Suspense)

## Next Steps
- Apply patterns learned here (schema design, auth flow) to future projects.
