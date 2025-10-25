# AI Agent Belgium

This repository contains a static front-end and a minimal backend proxy for OpenAI GPT-4.

Form

<form action="https://formspree.io/f/id" method="POST">

Replace `id` with your actual Formspree form ID (e.g. `f/abcd1234`).

Backend

A minimal Express backend has been added under /server to proxy requests to the OpenAI API. Do NOT commit your OPENAI_API_KEY to the repository. Use environment variables or your hosting platform's secrets.

How to run the backend locally

1. cd server
2. copy .env.example to .env and set OPENAI_API_KEY and FRONTEND_ORIGIN
3. npm install
4. npm run start

Hosting

- Front-end: Enable GitHub Pages (Settings → Pages → Branch: main, Folder: / (root)).
- Backend: Host the /server folder on Render, Vercel (as serverless), Heroku, etc. Set OPENAI_API_KEY in the host's environment variables and set FRONTEND_ORIGIN to your GitHub Pages domain.