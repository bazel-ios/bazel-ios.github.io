# bazel-ios.github.io

This repo shouldn't copy `rules_ios` or take away from the mono-repo spirit -
it's mainly a github pages convenience and this site might end up linking to
generated docs there. 

### How to contribute 

The site uses octopress. When you land a PR it generates the site. You can run
it locally:
```
bundle exec jekyll serve
```

For more info, see
https://github.com/imathis/octopress

### Known issues

1. `rules_ios` contains the canonical mono-repo and documentation for how to
build an iOS application with Bazel. This said, `rules_ios` needs critical fixes
to user level documentation: most of the stuff in the markdown files shouldn't
be in there and we should cut it to a tailored subset of how to use
`apple_framework` and `xcodeproj` rules.

2. We want to demonstrate impact and that `rules_ios` has became the defacto way
to build iOS with Bazel at scale. At this point, it's been widely used and
without such a site - everyone in the community knows the repos. However, in
order to further capture impact, we might want to add more bits to "impact"
segment but potentially need to vet them. To bootstrap this, I quoted Bazel blog
posts without editorializing them. Please file an issue or fix it if you'd like
to change one of these or no longer use Bazel.