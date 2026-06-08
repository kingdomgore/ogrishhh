# ogrish.lol

Free, customizable link-in-bio pages. Built with Next.js + Supabase.

## Setup

### 1. Install dependencies

```bash
npm install
```

### 2. Supabase

1. Create a project at [supabase.com](https://supabase.com)
2. Run the SQL in `supabase/schema.sql` in the Supabase SQL Editor
3. Copy `.env.local.example` to `.env.local` and fill in your keys:

```
NEXT_PUBLIC_SUPABASE_URL=https://xxxx.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
```

Find these in Supabase → Project Settings → API.

### 3. Run locally

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Pages

| Route | What |
|-------|------|
| `/` | Home — sign up / log in |
| `/signup` | Create account (free) |
| `/login` | Log in |
| `/dashboard` | Edit your page |
| `/[username]` | Public link page |

## Stack

- Next.js 15 (App Router)
- Supabase Auth + Postgres
- Tailwind CSS 4
