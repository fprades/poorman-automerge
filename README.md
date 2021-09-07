# poorman-devops

This is the Poorman devops. It automatically merges Pull Requests if all the previous steps complete successfully. Enforcing _build+tests_ in addition to the usual code merge conflict integrity.

- It checkouts the `head` branch
- Rebases `head` on top of `base` branch
- Runs the usual *build*, and *tests*.
- Pushes `head` and `base`, if all the previous conditions succeded. Effectivily merging the Pull Request

This is useful if you are running a limited, old, or restricted git hosting provider. For example auto-merge is not available on private github.com Free repositories.
