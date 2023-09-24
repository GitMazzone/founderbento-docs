---
sidebar_position: 1
---

# Start here

Let's discover **FounderBento in less than 5 minutes**.

## Clone the repo

```bash
git clone https://github.com/GitMazzone/founderbento-repo.git <your-app-name>
cd <your-app-name>
npm i
git remote remove origin
npm run dev
```

## Make a Supabase project

### On Supabase

...

### Update .env

Rename `.env.local.example` to `.env.local`.  
Do not check this file in. It is already in `.gitignore`.  

Add your Supabase info to `.env.local`:
```bash
# https://app.supabase.com/project/_/settings/api
NEXT_PUBLIC_SUPABASE_URL=https://<your-supabase-url>.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=<your-supabase-anon-key>
```

## Run locally

```bash
npm run dev
```

🥂 Visit `localhost:3000`!

## An overview of these docs

Now that you're running locally, the next sections will familiarize you with the repo and the awesome tooling at your disposal.  
TODO: brief overview of tour, quickstart, components, tools.
