# Profile README Editing Notes

This repo renders as the public GitHub profile README.

## Links To Sibling Repositories

Do not use relative links such as `../some-repo` for sibling GitHub
repositories in `README.md`. On the rendered profile page, GitHub can resolve
those links against the profile repo branch/tree context and produce broken
branch/tree URLs.

Use absolute GitHub URLs for sibling repos instead. If the public-safety hook
blocks adding the raw local username string, use the URL-encoded owner form:

```markdown
[Project](https://github.com/%67eorgewangyu/project-name)
```

GitHub resolves that URL correctly, and it avoids the local hook false positive.
