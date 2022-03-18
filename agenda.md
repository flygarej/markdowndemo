# Demo github migration

## Agenda

### Git migration bitbucket->github
#### Quick recap git
  - git/svn
  - git repo/bare repo
#### git local/git remote
  - add/commit -> local
  - pull/fetch/push -> remote
  - branches/tags in local/remote
#### multiple remotes
#### migration steps
  - mirror repo on bitbucket to local host
  - verify that local repo have all branches/tags
  - (optional) close bitbucket repo for writing
  - add github as new remote
  - push --all to github remote
  - check in github that repo looks ok including branches/tags
  - (optional) keep local repo if you need to sync bitbucket->github again
  - Make regular clone of new github repo, check it looks ok
  - set up collaborators in github repo

### Github features
#### organisations
Organisations allow us to have our own projects securely separate from organisation/company projects.
You can easily switch from your personal github account into the organisational one, making a context switch wrt to access rights at the same time.
#### tokens
Tokens allow us to give rights tools (IDE's, scripts etc) to access repos within an organisation
#### repositories
A repository is the basic unit for versioning a code project.
#### issues
Every repository can have and handle issues. It's possible to sync issues with JIRA if needed.
#### projects
A project can be defined on top of one or more repositories and provide a canban board to handle the issues in the repos, as well as a wiki for project-level documentation and a chat board for the members.
#### teams
Teams contain members and can be used to handle access to projects and repositories.
#### markdown
All documentation uses Github markdown. Mermaid capabilities was added recently
#### actions
Github actions allow us to act on push/pull request and merge in a repository.
This can be used in the same manner as Jenkins, to perform a build and flag broken commits to the repo/project/team
#### pull requests
Github assumes work is normally done in branches which are then merged into master via pull requests.
