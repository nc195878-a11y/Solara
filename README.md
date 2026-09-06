# Solara Journey

Build a working Solara emotional-wellness web app from the attached MVP specification. Deliver the full responsive MVP flow: onboarding with clear AI disclosure, home, daily mood check-in, contextual AI conversation with the three suggested actions, guided journal, reflections/insights, mood/activity patterns, wellness activities, and settings/privacy. Enable Lovable Cloud first for auth and persistent user data, and use Lovable AI for safe in-app AI functionality. Seed polished demo content so it is complete even before setup. Apply all specified safety boundaries: non-clinical positioning, persistent disclosure, crisis escalation screen and configurable support-resource copy, no diagnoses or dependency cues, privacy/deletion controls. Use the spec’s calm premium visual system and make it polished on mobile and desktop.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/285a8862-e1e6-47c7-838e-8b6c8cfe1c7a).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```

For local Supabase-backed development, provide `VITE_SUPABASE_URL` and
`VITE_SUPABASE_PUBLISHABLE_KEY` in `.env.local`. Server-side AI responses use
`GEMINI_API_KEY`. You may also set `GEMINI_MODEL`; it defaults to
`gemini-3.6-flash`.

The local app runs at `http://localhost:3000` so Supabase Google OAuth and
email-confirmation redirects return to the development server.

The configured Supabase project is `mgcvwzqvoaneblcwapww`. Its dashboard is
available at https://supabase.com/dashboard/project/mgcvwzqvoaneblcwapww.
Signed-in users' profiles, settings, check-ins, conversations, messages,
journals, activity logs, and insights are stored there. Anonymous demo content
is stored only in this browser's `localStorage` and is never uploaded to
Supabase.

The daily reminder uses browser notifications while the app is open. Marketing
emails are not offered until an email delivery service is connected.
