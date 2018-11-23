# How to contribute to this project

The `alphanet` branch is used for production releases and `develop` is the next release branch. Please work off of develop.

### Setup

1. Clone this repo to your local development machine
2. Checkout the `develop` branch

### Working on new features

1. Create a branch with a feature name using `git checkout -b {feature_name}`
2. Work on the changes locally to add in the feature.
3. Commit and push changes to the same branch on the origin.
4. Verify that all stages in CI (preconf, build and test) pass.
5. Use GitHub to raise a Pull Request and set one or more reviewers.
6. Respond to any comments as appropriate and make changes.
7. When all comments are dealt and the PR finally gets a :+1: from someone else then merge your PR into develop.
8. Test that the changes work on the develop resource group
9. Delete your feature branch and the corresponding resource group

### Features

Features must be named per the following pattern `#{issue number}/{some_descriptive-text}` — so for example, if you are working on issue `ABC-1` with the title "do the thing", call your feature `ABC-1/do_the-thing`. Obviously use your common sense to avoid making the feature names too long.

### Commit Messages

When committing something use the `-m` flag to add a short commit message of the format `{issue number} summary of what you changed`.  So for example if you are working on issue `ABC-1` and you added a method to the `aardvark_controller` you might use the following commit message `"ABC-1 added anteater method to aardvark controller"`

Commit messages ought to be in the past tense.

### Pull Requests

Pull requests must be named as follows `[issue type, issue number] high level description of change`.  The following Issue Types are recognized

* `Bug Fix` - the change fixes a bug
* `Feature` - the change adds a new feature (the usual issue type)
* `Documentation` — The change is a documentation only change
* `Optimisation` - The change is an optimisation of the code base without any functional changes

If your change does not fit any of these categories, use `Feature`. Likewise if your change is not tied to an issue number you may use `n/a` instead.

So to use the above example your Pull Request would be named `[Feature, ABC-1] added anteater to aardvark`

### You built it, you merge it

A developer must be responsible for their own work, from accepting a task through to merging to production.  With that in mind if you review another developer's PR, please don't then merge it yourself.  As a general rule you must let the developer merge her own PRs.

Likewise, don't expect someone else to merge your PR.  Unless you do not have write permission on a project, you will always aim to take personal responsibility for the quality of the code that gets merged in.
