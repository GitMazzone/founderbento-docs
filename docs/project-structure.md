---
sidebar_position: 2
---

# ⛩️ Project structure

This repo aims to be as standard as possible, not a bespoke new architecture you have to learn.  

For an in-depth understanding of NextJS repo structure, reference the [NextJS docs](https://nextjs.org/docs/getting-started/project-structure) as you go.  

You'll work with each of these in the tutorials to follow.

## Key directories

[/app](https://nextjs.org/docs/app/building-your-application/routing) - Replaces the old Pages router, built on [React Server Components](https://nextjs.org/docs/app/building-your-application/rendering/server-components). Your pages will live here!  
/components  
/config - App-wide config to save editing dozens of files. [More on this below](#config).  
[/public](https://nextjs.org/docs/app/building-your-application/optimizing/static-assets) - Static assets, like images.  
/styles - Minimal, global styles. All other CSS is inline or in a module alongside the component.  
/supabase - Database schema and seeds.  
/templates - Handlebars templates for use by [Plop](https://plopjs.com/) to generate components and pages.  

## Files  

`.env` - Environment variables.  
`.env.local` - Local environment variables.  
[`layout.tsx`](https://nextjs.org/docs/app/api-reference/file-conventions/layout) - Layout UI shared between routes. Also where we set font(s) and wrap our app with the `<AuthProvider>`.  
[`page.tsx`](https://nextjs.org/docs/app/api-reference/file-conventions/page) - UI for a given route.  
[`loading.tsx`](https://nextjs.org/docs/app/api-reference/file-conventions/loading) - UI for loading state of a given route.  
[`not-found.tsx`](https://nextjs.org/docs/app/api-reference/file-conventions/not-found) - UI that shows when a given route throws with the [notFound](https://nextjs.org/docs/app/api-reference/functions/not-found) function.  
[`error.tsx`](https://nextjs.org/docs/app/api-reference/file-conventions/error) - UI error boundary to catch unexpected errors and display a fallback.  
[`route.ts`](https://nextjs.org/docs/app/api-reference/file-conventions/route) - The new way to make API routes! Put a `route.ts` file inside of an `/app` folder.  

## Config

`config.ts` - Variables used throughout the app, like your app's display name.  
`routePaths.ts` - Routes. Common uses included in the file.  
`seoMetadata.ts` - Imported in the root-level `layout.tsx`. This is the new way to add SEO metadata in a NextJS project (previously in the `<Head>` in a page).  
