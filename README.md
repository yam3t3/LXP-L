# Linea User Points Logger

This repository contains a GitHub Actions workflow that logs user points data daily from a specified API endpoint. The data is appended to a CSV file, `log.csv`, allowing you to track key metrics over time.

## Workflow Setup

1. **Location**: The workflow file (`log-user-points.yml`) should be located in `.github/workflows/` within this repository.

2. **Permissions**:
   - Go to **Settings** > **Actions** > **General** in your repository.
   - Under **Workflow permissions**, select **Read and write permissions** to enable the workflow to push changes.

## How It Works

- **Schedule**: This workflow runs daily at midnight (UTC) or can be manually triggered from the Actions tab.
- **Data Logging**: The workflow fetches JSON data from the API endpoint and logs specified fields as a new row in `log.csv`.

## Manual Testing

To test the workflow manually:
1. Go to the **Actions** tab in your repository.
2. Select **Linea User Points Logs**.
3. Click **Run workflow** and confirm.

Check the repository for `log.csv` to see the logged data.

## Forking the Repository

If you fork this repository:
- The workflow will not run automatically on the fork unless you configure it to do so. 
- You may need to set the same permissions as in the original repository for the workflow to function correctly.
---
