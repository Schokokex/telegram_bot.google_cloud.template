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

# Finally.
Check if Build worked (if not, open Google Cloud Terminal in browser, type ```gcloud functions deploy foo-1 --region=europe-west3```...)

Open Link from Google Cloud Functions (goto Triggers) e.g. https://europe-west3-project-1.cloudfunctions.net/foo-1
