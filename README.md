# poorman-automerge

This is the _poorman automerge_. It automatically merges Pull Requests if all the previous steps complete successfully. Enforcing _build+tests_ in addition to the usual code merge conflict integrity.

- It checkouts the `from` branch.
- Rebases `from` on top of `into` branch.
- Runs the usual *build*, and *tests*.
- Pushes `form` and `into`, if all the previous conditions succeded. Effectivily merging the Pull Request

This is useful if you are running a limited, old, or restricted git hosting provider. For example auto-merge is not available on private github.com free repositories.

More info: https://www.linkedin.com/posts/fprades_poorman-automerge-building-automerge-in-activity-6841120146187268096-ZQC1
