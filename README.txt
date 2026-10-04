WaseemSial Milk Collection Center - Cloud Accounts

What this version does:
- Stores purchase, sale and milk-rate data in a Supabase cloud database.
- Login/signup with email + password.
- Same data can be opened on phone, tablet or computer after login.
- User data is protected by Supabase Row Level Security (each account sees its own records).
- Export/import backup is included.

SETUP
1. Create a Supabase project at https://supabase.com/
2. Open SQL Editor -> New query.
3. Paste ALL contents of supabase-schema.sql and click Run.
4. In Supabase, open Settings -> API Keys (or Connect) and copy the Project URL and Publishable key.
5. Open index.html in a text editor and replace:
   YOUR_SUPABASE_URL
   YOUR_SUPABASE_PUBLISHABLE_KEY
   with your project's values.
   Never put a service_role/secret key in index.html.
6. Upload the updated index.html and the image files to GitHub Pages, replacing the old files.
7. Open the website, create your account, and sign in.

NOTES
- Supabase's browser client uses the project URL and publishable key; database access is secured by RLS policies.
- The website does not need your Supabase password.
- If email confirmation is enabled in Supabase Auth, confirm the signup email before logging in.
