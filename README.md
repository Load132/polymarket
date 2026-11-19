# Class Forecasts — setup
1. Create a Supabase project. In the SQL editor, run `supabase/migrations/001_schema.sql`.
2. Copy `.env.example` to `.env.local` and fill in your project URL and anon key.
3. `npm install && npm run dev`
4. Sign up with your own email, then in the SQL editor run:
   `update public.users set role='admin' where email='YOUR@EMAIL';`
5. Students sign up; on /admin press "Send 1,000 credits", create a market, open it.
Lifecycle: draft → open → locked → resolved (payouts happen on resolve).
