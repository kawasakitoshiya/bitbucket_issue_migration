# bitbucket Issues Migration

This is a small script that will migrate bitbucket issues to a github project.
It will use the bitbucket api to pull out the issues and comments.

It will import issues (and close them as needed) and their comments. Labels and
milestones are not supported at the moment.

## Before running

You will need to install the requirements first

    pip install -r requirements.pip

## Example

```
python migrate.py <your_bitbucket_username> <bitbucket_org/bitbucket_repo> <your_github_username> <github_org/github_repo>
```

Note: if you need to migrate to a GitHub organizational repository, use your personal username,
but the appropriate API token for the repository.
