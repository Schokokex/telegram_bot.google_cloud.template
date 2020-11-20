# 0. Create github repo (fork)
# 1. Create Google Project
goto cloud.google.com
create new Project
# 2. Mirror repo
goto Google Cloud Source Repositories in Google cloud
add Repository (to right)
external Repo
select Project and github repo
(click connect to other repo on fail and check checkbox)
# 3. Create build trigger
goto Google Cloud Build
click Connect Repository
select Github (first)
Install Cloud Build App into the github Repo, just the one
check, check
create Push trigger
# 4. Give rights to build trigger (Cloud Build Settings)
Set (everything? / Functions?) to activated
# 5. Edit cloudybuild.yaml
foo-1: function name in Google Functions
project-1: project id
github_schokokex_template-bot-gcloud: mirrored repo
