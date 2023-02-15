## Github Actions: 

- HashiCorp configuration language.
- Docker everything 
- 2018 sept 
- Matrix builds 
- No native caching, no support for forks, linux distro

Workflow, Job, Step, Action 

* 20 workflows concurrently per repository.
* 1000 API requests in an hour across all actions within a repository.
* Each job in a workflow can run for up to 6 hours of execution time.
* You can run up to 20 jobs concurrently per repository across all workflows.


don’t use GitHub Actions in ways you know you shouldn’t.


* applypatch-msg
* pre-applypatch
* post-applypatch
* pre-commit
* prepare-commit-msg
* commit-msg
* post-commit
* pre-rebase
* post-checkout
* post-merge
* pre-receive before starting to update refs on the remote repository
* update
* post-receive 
* post-update
* pre-auto-gc Cleanup unnecessary files and optimize the local repository
* post-rewrite
* pre-push
