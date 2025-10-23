Create a scheduled GitHub action that runs daily and adds a commit to your repository. The workflow should:

Use schedule with cron syntax to run once per day (must use specific hours/minutes, not wildcards)
Include a step with your email 23f1002487@ds.study.iitm.ac.in in its name
Create a commit in each run
Be located in .github/workflows/ directory
After creating the workflow:

Trigger the workflow and wait for it to complete
Ensure it appears as the most recent action in your repository
Verify that it creates a commit during or within 5 minutes of the workflow run