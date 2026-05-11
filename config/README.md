# Configuration Guide

## Users Configuration

Edit `users.json` to add your Codeforces and AtCoder usernames:

```json
{
  "codeforces": ["username1", "username2"],
  "atcoder": ["username1", "username2"]
}
```

### Current Configuration

- **Codeforces**: Ayon
- **AtCoder**: AyonCoder

## How to Update Usernames

1. Edit `config/users.json`
2. Update the usernames under each platform
3. Commit and push to trigger the workflow
4. GitHub Actions will fetch submissions automatically

## Harwest Workflow

The GitHub Actions workflow runs:
- **Automatically**: Every day at 11:00 PM BDT (5:00 PM UTC)
- **Manually**: Go to Actions → Run workflow (with optional full scan)

### Workflow Features

- Downloads submissions from your profiles
- Organizes them by contest/problem
- Generates markdown tables (codeforces.md, atcoder.md)
- Automatically commits and pushes changes
- No additional configuration needed!
