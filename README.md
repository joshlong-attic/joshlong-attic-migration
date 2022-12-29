# A Script to Generate the Commands that Automated Moving Repositories from `joshlong` to `joshlong-attic`.

This is a hacky bit of code that I used to code-generate the commands to move everything to this new Github organization. (You didn't think I was going to manually move more than 500 Github repositories, did you?)


You'll need to define an environment variable called `GH_PAT` which contains the Github Personal Access Token you want to use to run this script, as it in turn uses `curl` to call the Github REST API.

This script prints out the commands to migrate the application from one organization to another.  Run this script (`pipenv run python main.py`), direct the output to a a file, say `run.sh`, then make that script executable (`chmod a+x run.sh`), then run it: `./run.sh`. 
