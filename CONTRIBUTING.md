# Contributing

All changes to company code should be made through pull requests.

## Development workflow

1. Create a branch from the latest `main`.
2. Make and test your changes locally.
3. Open a pull request into `main`.
4. Obtain at least one approval.
5. Resolve all review comments and ensure required checks pass.
6. Squash merge the pull request into `main`.

Direct pushes to `main` should not be used.

## Branches

Use short-lived branches for development.

Branches should normally be deleted after their pull request is merged.

## Pull requests

Pull requests should:

* explain what changed and why;
* be small enough to review effectively where practical;
* include or update tests when behavior changes;
* identify any known limitations or follow-up work;
* pass all required automated checks before merging.

Draft pull requests may be opened for work that is not yet ready to merge.

## Reviews

At least one approval is required before merging into `main`.

Reviewers should consider correctness, maintainability, tests, and any relevant numerical or performance implications.

Substantial changes to another developer's area of ownership should involve that developer in the review where practical.

## Commits and merging

Development commits may be incremental and do not need to form a polished permanent history.

Pull requests are squash merged so that `main` contains one meaningful commit for each merged change.

The squash commit message should clearly describe the change.

## Testing

Changes should include appropriate testing for the behavior they affect.

At minimum, existing tests should continue to pass. Changes to numerical algorithms should include appropriate numerical validation or regression tests where applicable.

Do not merge known failing tests into `main` unless there is an explicit and documented reason.

## Security

Do not commit credentials, API keys, private keys, `.env` files, tokens, or other secrets to a repository.

See `SECURITY.md` for security-related procedures.
