# 0. Create github repo (fork)
# 1. Create Google Project
goto cloud.google.com
create new Project
# 2. Mirror repo
goto Cloud Source Repositories in Google cloud
add Repository (to right)
external Repo
select Project and github repo
(click connect to other repo on fail and check checkbox)
# 3. Create build trigger
# 4. Give rights to build trigger (Build Settings)
# 5. Edit cloudybuild.yaml
cloudy-foo: function name in Google Functions
project-1: project id
github_schokokex_template: mirrored repo
