# Postgres Setup

This repository is meant to own its own dedicated Postgres database, separate from the larger publishing pipeline.

## Recommended Provisioning Path

Use a Vercel-managed Neon Postgres database attached directly to the Vercel project `dayton-visual-database`.

That gives this repo:

- its own isolated database
- auto-generated Postgres environment variables in Vercel
- a clean separation from the rest of the pipeline
- an easy path to productionize later

## Expected Environment Variables

Once provisioned, the Vercel project should contain:

- `POSTGRES_URL`
- `POSTGRES_NON_POOLED_URL`

## Local Development

After the database is attached to the Vercel project, pull the values locally into `.env.local` and keep secrets out of git.

## Notes

- Do not commit real database URLs or passwords into the repository.
- `.env.example` exists only as a contract for future implementation work.
