### Restore deleted file

git restore --source=origin/main -- LICENSE

### Pull Request

## ================================================================================

1. Find the key for the Jira work item you want to link to, for example “JRA-123”.
   You can find the key in several places in Jira:

• On the board, work item keys appear at the bottom of a card.
• On the work item’s details, keys appear in the breadcrumb navigation at the top of the page.

Find out about work item keys.

## ================================================================================

2. Check out a new branch in your repo, using the key in the branch name.
   For example, git checkout -b JRA-123-<branch-name>.

## ================================================================================

3. When committing changes to your branch, use the key in your commit message
   to link those commits to the development panel in your Jira work item.
   For example, git commit -m "JRA-123 <summary of commit>".

## ================================================================================

4. When you create a pull request, use the key in the pull request title.

## ================================================================================

Connecting GitHub to Jira allows you to view development activity in the context of
your Jira project and issues. To send development data from GitHub to Jira,
your team must include issue keys in branch names, commit messages, and pull request titles.
Even if your organization is still backfilling historical data, you can start using issue keys
in your development work immediately.
