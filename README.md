# Github_Traffic_Cop
Patrolling my Github Traffic and telling me what happens


# GitHub Traffic Cop 🚦👮‍♀️

GitHub Traffic Cop is an AI-powered traffic tracker for GitHub repositories.

GitHub shows repo traffic for a limited window, but this app saves regular snapshots so you can track views, clones, referrers, and popular files over time.

> 🚨 Pull over. Your repo is getting attention.

## What It Does

- Tracks repo views
- Tracks unique visitors
- Tracks clones
- Tracks unique cloners
- Tracks top referrers
- Tracks popular paths/files
- Saves daily snapshots
- Detects traffic spikes
- Generates AI traffic summaries

## Important Privacy Note

GitHub does not show exactly who visited your repo.

GitHub Traffic Cop tracks activity trends, not individual people. It does not collect names, usernames, emails, or IP addresses.

## Why I Built This

I wanted a fun way to monitor traffic across my GitHub projects after sharing them on LinkedIn, Discord, resumes, portfolios, and demos.

Instead of manually checking GitHub Insights every few days, GitHub Traffic Cop saves the data and summarizes what changed.

## Tech Stack

- Frontend: React + Chakra UI
- Backend: Node.js + Express
- Database: PostgreSQL
- API: GitHub REST API
- AI: OpenAI API
- Deployment: Railway / Vercel

## GitHub Data Used

GitHub Traffic Cop uses GitHub’s repository traffic API to collect:

- Views
- Clones
- Top referrers
- Popular paths

## Planned Features

- GitHub personal access token setup
- Add one or more repositories
- Daily traffic snapshot job
- Dashboard with repo cards
- Weekly AI traffic report
- Traffic spike alerts
- Referrer summaries
- Clone activity summaries
- “Incident report” style AI summaries

## Example AI Summary

> 🚨 Traffic Report: Sexy Phish received 42 views this week, with most traffic coming from LinkedIn. Clone activity increased after your latest post, suggesting people may be testing or reviewing the project.

## Example Dashboard

Each repo card could show:

- Total views
- Unique visitors
- Total clones
- Unique cloners
- Top referrer
- Most viewed file
- Traffic trend
- AI summary

## Database Plan

### users

Stores app users.

```sql
id
github_username
created_at
