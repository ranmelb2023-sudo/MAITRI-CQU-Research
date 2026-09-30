# MAITRI CQUniversity Research Website

## Architecture
- `index.html` — public website
- `data/content.json` — editable content for the current static version
- `admin.html` — starter admin/help page
- `supabase-schema.sql` — database schema for the next stage
- `reference_static_homepage.html` — original static prototype

## Publish the current version
The site can be hosted with GitHub Pages because GitHub Pages publishes HTML/CSS/JavaScript from a repository. Create a GitHub repository, upload this folder, then enable Pages under repository Settings > Pages.

## Edit content now
Edit `data/content.json`, commit the change, and GitHub Pages will publish the updated site.

## Database stage
For a real database-backed admin system, create a Supabase project, run `supabase-schema.sql` in the SQL Editor, configure Supabase Auth for authorised administrators, and then connect the public website/admin dashboard to the Supabase Data API. Keep service-role secrets on a server; never expose them in public browser code.

## Suggested future tables
project_settings, objectives, methodology, research_questions, researchers, roadmap, publications, news, datasets, documents, experiments, results.
