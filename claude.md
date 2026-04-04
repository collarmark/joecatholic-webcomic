# Joe Catholic — Claude Code Context

## What This Is
Joe Catholic is a Catholic webcomic site built on Jekyll, managed with Decap CMS, 
and deployed via Netlify from a GitHub repository. The comic follows Joe Catholic 
on adventures through faith and time.

## Stack
- **Static site generator:** Jekyll
- **CMS:** Decap CMS (config at `admin/config.yml`)
- **Deployment:** Netlify, auto-deploy from GitHub `main` branch
- **Markdown:** kramdown

## Collections
- `_comics/` — Individual comic strip entries. Each has an image, commentary, 
  transcript, characters, and tags.
- `_posts/` — Blog posts with full markdown body content.
- `_tutorials/` — Tutorial entries tied to YouTube videos, with metadata like 
  difficulty, duration, and downloadable resources.
- `_explores/` — Joe Catholic Explores catechetical archive. PDF and interactive 
  resources for K-8 students.

## Decap CMS Notes
- Config is at `admin/config.yml`
- Characters and tags fields use a single-field list widget to allow spaces in names.
  Do not simplify these to a plain list widget or it will break.
- Preview pane is disabled. This is intentional.
- Media folders are collection-specific. Check existing config before changing paths.

## Conventions
- Slugs follow `YYYY-MM-DD-title` format.
- Front matter uses Jekyll defaults defined in `_config.yml`. Do not add layout 
  fields manually unless the hidden widget is already present.
- Timezone is America/Chicago.

## Deployment
- Push to `main` triggers an automatic Netlify build.
- Do not commit directly to `main` for experimental changes. Use a branch.

## Author
Fr. Christopher J. Decker — pastor, cartoonist, and content creator. 
Site is maintained by a non-developer. Keep solutions simple and well-explained.