# dayton_visual_database

Placeholder repository for a productionizable visual database service in a larger autonomous publishing pipeline.

For now, this repo is intentionally thin. The immediate goal is to reserve its own GitHub repo, Vercel project, and dedicated Postgres contract so it can be built out later without reopening the wider pipeline architecture.

## Planned Role

This project will eventually become a Cloudinary-backed image and video database that feeds a larger autonomous article writing and publishing system.

## Current Infrastructure Status

- GitHub repository connected
- Vercel project linked
- Postgres environment contract defined
- No application code scaffolded yet by design

## Postgres Contract

When the database is provisioned, the project should receive these environment variables:

- `POSTGRES_URL`
- `POSTGRES_NON_POOLED_URL`

See `docs/postgres-setup.md` for the intended setup.
