# TDS-GA5-Q8 - Daily Commit GitHub Action

This repository contains a scheduled GitHub Action that automatically creates daily commits.

[![Daily Commit Scheduler](https://github.com/23f1002487/TDS-GA5-Q8/actions/workflows/daily-commit.yml/badge.svg)](https://github.com/23f1002487/TDS-GA5-Q8/actions/workflows/daily-commit.yml)

## Workflow Details

- **Schedule**: Runs daily at 11:15 AM UTC using cron syntax `15 11 * * *`
- **Purpose**: Creates automated daily commits to maintain repository activity
- **Email**: Configured for 23f1002487@ds.study.iitm.ac.in
- **Files Created**: 
  - `daily_commits.log` - Log of all daily commits
  - `last_run.txt` - Timestamp of the last workflow run

## Workflow Features

1. **Scheduled Execution**: Uses GitHub Actions cron scheduler with specific time (not wildcards)
2. **Email Integration**: Step names include the specified email address
3. **Automated Commits**: Creates meaningful commits with timestamps
4. **Manual Trigger**: Can be manually triggered via workflow_dispatch
5. **Verification**: Includes steps to verify commit creation

## Files Generated

- `daily_commits.log`: Contains a log entry for each daily commit
- `last_run.txt`: Contains the timestamp of the last workflow execution

## How it Works

1. The workflow checks out the repository
2. Configures Git with the specified email
3. Creates/updates log files with current timestamp
4. Commits and pushes the changes
5. Verifies the commit was created successfully

## Manual Trigger

You can manually trigger this workflow from the GitHub Actions tab by clicking "Run workflow" on the "Daily Commit Scheduler" workflow.
