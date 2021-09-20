# poorman-automerge

This is the _poorman automerge_. It automatically merges Pull Requests if all the previous steps complete successfully. Enforcing _build+tests_ in addition to the usual code merge conflict integrity.

- It checkouts the `from` branch.
- Rebases `from` on top of `into` branch.
- Runs the usual *build*, and *tests*.
- Pushes `form` and `into`, if all the previous conditions succeded. Effectivily merging the Pull Request

This is useful if you are running a limited, old, or restricted git hosting provider. For example auto-merge is not available on private github.com free repositories.

More info: [linkedin post](https://www.linkedin.com/feed/update/urn:li:ugcPost:6841120145868513281?updateEntityUrn=urn%3Ali%3Afs_feedUpdate%3A%28*%2Curn%3Ali%3AugcPost%3A6841120145868513281%29)
